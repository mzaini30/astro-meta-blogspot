# Astro Meta Blogspot

Example:

```astro
---
import Meta from 'astro-meta-blogspot'
---

<!DOCTYPE html>
<html lang="en">
<head>
	<Meta></Meta>
</head>
<body>
	
</body>
</html>
```

Result:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <include expiration="7d" path="*.css"></include>
    <include expiration="7d" path="*.js"></include>
    <include expiration="3d" path="*.gif"></include>
    <include expiration="3d" path="*.jpeg"></include>
    <include expiration="3d" path="*.jpg"></include>
    <include expiration="3d" path="*.png"></include>
    <meta content="sat, 10 jul 2021 00:00:00 GMT" http-equiv="expires">
    <meta charset="utf-8">
    <meta content="width=device-width, initial-scale=1, user-scalable=no" name="viewport">
    <meta content="blogger" name="generator">
    <meta content="text/html; charset=UTF-8" http-equiv="Content-Type">
    <link href="https://www.blogger.com/openid-server.g" rel="openid.server">
    <link expr:href="data:blog.homepageUrl" rel="openid.delegate">
    <link expr:href="data:blog.url" rel="canonical">
    <b:if cond="data:view.isMultipleItems">
        <title>
            <data:blog.pageTitle></data:blog.pageTitle>
        </title>
        <b:else></b:else>
        <b:if cond="!data:view.isError">
            <title>&#8730; <data:blog.pageName></data:blog.pageName> - <data:blog.title></data:blog.title>
            </title>
        </b:if>
    </b:if>
    <b:if cond="data:view.isError">
        <title>Page Not Found - <data:blog.title></data:blog.title>
        </title>
    </b:if>
    <b:if cond="data:view.isArchive">
        <meta content="noindex,noarchive" name="robots">
    </b:if>
    <b:if cond="data:blog.searchQuery">
        <meta content="noindex,noarchive" name="robots">
    </b:if>
    <b:if cond="data:blog.searchlabel">
        <meta content="noindex,noarchive,nofollow" name="robots">
    </b:if>
    <b:if cond="data:blog.isMobile">
        <meta content="noindex,nofollow" name="robots">
    </b:if>
    <b:if cond="!data:view.isError">
        <meta expr:content="data:blog.metaDescription" name="description">
        <script type="application/ld+json">
        { & quot;
            @context & quot;: & quot;
            https: //schema.org&quot;, &quot;@type&quot;: &quot;WebSite&quot;, &quot;url&quot;: &quot;<data:blog.homepageUrl/>&quot;, &quot;potentialAction&quot;: { &quot;@type&quot;: &quot;SearchAction&quot;, &quot;target&quot;: &quot;<data:blog.homepageUrl/>?q={search_term}&quot;, &quot;query-input&quot;: &quot;required name=search_term&quot; } }
        </script>
        <b:if cond="data:blog.homepageUrl != data:blog.url">
            <meta expr:content="data:blog.pageName + &quot;, &quot; + data:blog.pageTitle + &quot;, &quot; + data:blog.title" name="keywords">
        </b:if>
    </b:if>
    <b:if cond="data:blog.url == data:blog.homepageUrl">
        <meta content="DESKRIPSI-BLOG" name="keywords">
    </b:if>
    <link expr:href="data:blog.homepageUrl + &quot;feeds/posts/default&quot;" expr:title="data:blog.title + &quot; - Atom&quot;" rel="alternate" type="application/atom+xml">
    <link expr:href="data:blog.homepageUrl + &quot;feeds/posts/default?alt=rss&quot;" expr:title="data:blog.title + &quot; - RSS&quot;" rel="alternate" type="application/rss+xml">
    <link expr:href="&quot;https://www.blogger.com/feeds/&quot; + data:blog.blogId + &quot;/posts/default&quot;" expr:title="data:blog.title + &quot; - Atom&quot;" rel="alternate" type="application/atom+xml">
    <b:if cond="data:view.isPost">
        <b:if cond="data:blog.postImageThumbnailUrl">
            <link expr:href="data:blog.postImageThumbnailUrl" rel="image_src">
        </b:if>
    </b:if>
    <link expr:href="data:blog.url" hreflang="x-default" rel="alternate">
    <link href="/favicon.ico" rel="icon" type="image/x-icon">
    <link href="https://www.blogger.com/profile/USER-BLOGGER-ANDA" rel="publisher">
    <link href="https://www.blogger.com/profile/USER-BLOGGER-ANDA" rel="author">
    <link href="https://www.blogger.com/profile/USER-BLOGGER-ANDA" rel="me">
    <meta content="KODE-VALIDASI-GOOGLE-WEBMASTER" name="google-site-verification">
    <meta content="KODE-VALIDASI-BING-WEBMASTER" name="msvalidate.01">
    <meta content="Indonesia" name="geo.placename">
    <meta content="NAMA-ADMIN" name="Author">
    <meta content="general" name="rating">
    <meta content="id" name="geo.country">
    <b:if cond="data:view.isPost">
        <meta expr:content="data:blog.pageName" property="og:title">
        <meta expr:content="data:blog.canonicalUrl" property="og:url">
        <meta content="article" property="og:type">
    </b:if>
    <meta expr:content="data:blog.title" property="og:site_name">
    <b:if cond="data:blog.url == data:blog.homepageUrl">
        <meta expr:content="data:blog.metaDescription" name="description">
        <meta expr:content="data:blog.title" property="og:title">
        <meta content="website" property="og:type">
        <b:if cond="data:blog.metaDescription">
            <meta expr:content="data:blog.metaDescription" property="og:description">
            <b:else></b:else>
            <meta expr:content="&quot;Silakan kunjungi &quot; + data:blog.pageTitle + &quot; Untuk membaca postingan menarik Arlina Code.&quot;" property="og:description">
        </b:if>
    </b:if>
    <b:if cond="data:view.isPost">
        <meta expr:content="data:blog.metaDescription" property="og:description">
    </b:if>
    <b:if cond="data:blog.postImageUrl">
        <meta expr:content="data:blog.postImageUrl" property="og:image">
    </b:if>
    <meta content="https://www.facebook.com/PROFIL-FACEBOOK" property="article:author">
    <meta content="https://www.facebook.com/FAN-PAGE-FACEBOOK" property="article:publisher">
    <meta content="KODE-APLIKASI-FACEBOOK" property="fb:app_id">
    <meta content="KODE-ADMIN-FACEBOOK" property="fb:admins">
    <meta content="en_US" property="og:locale">
    <meta content="en_GB" property="og:locale:alternate">
    <meta content="id_ID" property="og:locale:alternate">
    <meta content="summary" name="twitter:card">
    <meta expr:content="data:blog.pageTitle" name="twitter:title">
    <meta content="USER-TWITTER" name="twitter:site">
    <meta content="USER-TWITTER" name="twitter:creator">
    <meta content="summary_large_image" name="twitter:card">
    <link href="//ajax.googleapis.com" rel="dns-prefetch">
    <link href="//www.google-analytics.com" rel="dns-prefetch">
    <link href="//googleads.g.doubleclick.net" rel="dns-prefetch">
    <link href="//www.googletagservices.com" rel="dns-prefetch">
    <link href="//pagead2.googlesyndication.com" rel="dns-prefetch">
    <link href="//maxcdn.bootstrapcdn.com" rel="dns-prefetch">
    <link href="//adservice.google.ca" rel="dns-prefetch">
    <link href="//adservice.google.com" rel="dns-prefetch">
    <link href="//resources.blogblog.com" rel="dns-prefetch">
    <link href="//fonts.googleapis.com" rel="dns-prefetch">
    <link href="//1.bp.blogspot.com" rel="dns-prefetch">
    <link href="//2.bp.blogspot.com" rel="dns-prefetch">
    <link href="//3.bp.blogspot.com" rel="dns-prefetch">
    <link href="//4.bp.blogspot.com" rel="dns-prefetch">
    <link href="//disqus.com" rel="dns-prefetch">
    <link href="//github.com" rel="dns-prefetch">
    <link href="//cdn.rawgit.com" rel="dns-prefetch">
    <link href="//fontawesome.com" rel="dns-prefetch">
    <link href="//www.sharethis.com" rel="dns-prefetch">
    <link href="//cdn.jsdelivr.net" rel="dns-prefetch">
    <link href="//youtube.com" rel="dns-prefetch">
    <link href="//cdn.statically.io" rel="dns-prefetch">
    <script>window.HMR_WEBSOCKET_PORT = 12321;</script>
    <script type="module" src="/_snowpack/hmr-client.js"></script>
</head>

<body></body>

</html>
```