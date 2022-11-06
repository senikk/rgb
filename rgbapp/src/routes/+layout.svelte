<script>
    import {
        Header,
        HeaderNav,
        HeaderNavItem,
        SkipToContent,
        Content
    } from "carbon-components-svelte";
</script>

<Header company="" platformName="VBUKLAN RGB" href="/">
    <div slot="skip-to-content">
        <SkipToContent />
    </div>
    <HeaderNav>
        <HeaderNavItem href="/" text="Veksle" />
        <HeaderNavItem href="/timer" text="Timer" />
    </HeaderNav>
</Header>

<Content>
    <slot></slot>
</Content>