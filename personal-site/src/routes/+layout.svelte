<script>
    import { page } from '$app/stores';
</script>




<div class="container-fluid text-center py-3">
    <div class="container">
        <nav>
            <div class="row text-center mb-4">
                <div class="col nav-item">
                    <a href="/" class:active={$page.url.pathname === '/'} aria-current={$page.url.pathname === '/'}>Home</a>
                </div>
                <div class="col nav-item">
                    <a href="/blog" class:active={$page.url.pathname === '/blog'} aria-current={$page.url.pathname === '/blog'}>Blog</a>
                </div>
                <div class="col nav-item">
                    <a href="/portfolio" class:active={$page.url.pathname === '/portfolio'} aria-current={$page.url.pathname === '/portfolio'}>Portfolio</a>
                </div>
            </div>
        </nav>
    </div>

    <slot />
</div>

<style>
    a.active {
        text-decoration-thickness: .1rem;
        font-weight: 550;
    }
</style>

<!-- 
<div class='row'>
    <div class='col-9'>col9</div>
    <div class='col-3'>col3</div>
</div>

<nav>
    <a href='/'>Home</a>
    <a href='/portfolio'>Portfolio</a>
    <a href='/blog'>Blog</a>
</nav>

<div id='content'>
    <slot></slot>
</div>


<style>

    :global(h1) {
        font-family: 'Courier New', Courier, monospace;
    }
</style> -->
