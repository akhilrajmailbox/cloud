



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-cfd028037d00b8a80c5a3b91967e29dcc41309e44d4ccece88663a52963ca765.css" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-dc8832cbc25013ebcdcca24529e402cfcea50e4b2bd136b8284fdf8864873636.css" media="all" rel="stylesheet" />
    
    
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/site-9e0f35305336555b58884b07a160747fc1f6dbd79e13e18820a598a9abcb2662.css" media="all" rel="stylesheet" />
    

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    <title>OpenStack-Juno-Installation/OpenStack-Juno-Installation.rst at master · ChaimaGhribi/OpenStack-Juno-Installation · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars1.githubusercontent.com/u/8246244?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="ChaimaGhribi/OpenStack-Juno-Installation" name="twitter:title" /><meta content="OpenStack-Juno-Installation - In this installation guide, we cover the step-by-step process of installing Openstack Juno on Ubuntu." name="twitter:description" />
      <meta content="https://avatars1.githubusercontent.com/u/8246244?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="ChaimaGhribi/OpenStack-Juno-Installation" property="og:title" /><meta content="https://github.com/ChaimaGhribi/OpenStack-Juno-Installation" property="og:url" /><meta content="OpenStack-Juno-Installation - In this installation guide, we cover the step-by-step process of installing Openstack Juno on Ubuntu." property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    
    <meta name="request-id" content="6A3327AD:0684:5D9E58C:5855001F" data-pjax-transient>

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="6A3327AD:0684:5D9E58C:5855001F" name="octolytics-dimension-request_id" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged Out">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="MzA2YjY0MTA0YzE1ZDViMzc5MmI1M2M3N2JlMmIwNTM3M2I5ZDg2Y2RmNmQwNWM4NWJmYzdlMTJkMjFjOTA0Mnx7InJlbW90ZV9hZGRyZXNzIjoiMTA2LjUxLjM5LjE3MyIsInJlcXVlc3RfaWQiOiI2QTMzMjdBRDowNjg0OjVEOUU1OEM6NTg1NTAwMUYiLCJ0aW1lc3RhbXAiOjE0ODE5NjU1OTksImhvc3QiOiJnaXRodWIuY29tIn0=">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#000000">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="7b264aa573e360504ba44e6705c41431f6c0f49b">
    <meta content="15b0151bc2f5772347f96dd6ac86c69d93a5a7b0" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="8cdbb8cffd6956425aaad8ad14e0496b">
    

      
  <meta name="description" content="OpenStack-Juno-Installation - In this installation guide, we cover the step-by-step process of installing Openstack Juno on Ubuntu.">
  <meta name="go-import" content="github.com/ChaimaGhribi/OpenStack-Juno-Installation git https://github.com/ChaimaGhribi/OpenStack-Juno-Installation.git">

  <meta content="8246244" name="octolytics-dimension-user_id" /><meta content="ChaimaGhribi" name="octolytics-dimension-user_login" /><meta content="31440267" name="octolytics-dimension-repository_id" /><meta content="ChaimaGhribi/OpenStack-Juno-Installation" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="31440267" name="octolytics-dimension-repository_network_root_id" /><meta content="ChaimaGhribi/OpenStack-Juno-Installation" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/ChaimaGhribi/OpenStack-Juno-Installation/commits/master.atom" rel="alternate" title="Recent Commits to OpenStack-Juno-Installation:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/ChaimaGhribi/OpenStack-Juno-Installation/blob/master/OpenStack-Juno-Installation.rst" data-pjax-transient>
  </head>


  <body class="logged-out  env-production  vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



          <header class="site-header js-details-container" role="banner">
  <div class="container-responsive">
    <a class="header-logo-invertocat" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="32" version="1.1" viewBox="0 0 16 16" width="32"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
    </a>

    <button class="btn-link float-right site-header-toggle js-details-target" type="button" aria-label="Toggle navigation">
      <svg aria-hidden="true" class="octicon octicon-three-bars" height="24" version="1.1" viewBox="0 0 12 16" width="18"><path fill-rule="evenodd" d="M11.41 9H.59C0 9 0 8.59 0 8c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zm0-4H.59C0 5 0 4.59 0 4c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zM.59 11H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1H.59C0 13 0 12.59 0 12c0-.59 0-1 .59-1z"/></svg>
    </button>

    <div class="site-header-menu">
      <nav class="site-header-nav site-header-nav-main">
        <a href="/personal" class="js-selected-navigation-item nav-item nav-item-personal" data-ga-click="Header, click, Nav menu - item:personal" data-selected-links="/personal /personal">
          Personal
</a>        <a href="/open-source" class="js-selected-navigation-item nav-item nav-item-opensource" data-ga-click="Header, click, Nav menu - item:opensource" data-selected-links="/open-source /open-source">
          Open source
</a>        <a href="/business" class="js-selected-navigation-item nav-item nav-item-business" data-ga-click="Header, click, Nav menu - item:business" data-selected-links="/business /business/partners /business/features /business/customers /business">
          Business
</a>        <a href="/explore" class="js-selected-navigation-item nav-item nav-item-explore" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship /showcases /explore">
          Explore
</a>      </nav>

      <div class="site-header-actions">
            <a class="btn btn-primary site-header-actions-btn" href="/join?source=header-repo" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
          <a class="btn site-header-actions-btn mr-1" href="/login?return_to=%2FChaimaGhribi%2FOpenStack-Juno-Installation%2Fblob%2Fmaster%2FOpenStack-Juno-Installation.rst" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
      </div>

        <nav class="site-header-nav site-header-nav-secondary mr-md-3">
          <a class="nav-item" href="/pricing">Pricing</a>
          <a class="nav-item" href="/blog">Blog</a>
          <a class="nav-item" href="https://help.github.com">Support</a>
          <a class="nav-item header-search-link" href="https://github.com/search">Search GitHub</a>
              <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/ChaimaGhribi/OpenStack-Juno-Installation/search" class="js-site-search-form" data-scoped-search-url="/ChaimaGhribi/OpenStack-Juno-Installation/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
    </label>
</form></div>

        </nav>
    </div>
  </div>
</header>



    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
      <a href="/login?return_to=%2FChaimaGhribi%2FOpenStack-Juno-Installation"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
  </a>
  <a class="social-count" href="/ChaimaGhribi/OpenStack-Juno-Installation/watchers"
     aria-label="9 users are watching this repository">
    9
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2FChaimaGhribi%2FOpenStack-Juno-Installation"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"/></svg>
    Star
  </a>

    <a class="social-count js-social-count" href="/ChaimaGhribi/OpenStack-Juno-Installation/stargazers"
      aria-label="26 users starred this repository">
      26
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2FChaimaGhribi%2FOpenStack-Juno-Installation"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
      </a>

    <a href="/ChaimaGhribi/OpenStack-Juno-Installation/network" class="social-count"
       aria-label="32 users forked this repository">
      32
    </a>
  </li>
</ul>

    <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a href="/ChaimaGhribi" class="url fn" rel="author">ChaimaGhribi</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/ChaimaGhribi/OpenStack-Juno-Installation" data-pjax="#js-repo-pjax-container">OpenStack-Juno-Installation</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/ChaimaGhribi/OpenStack-Juno-Installation" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /ChaimaGhribi/OpenStack-Juno-Installation" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/ChaimaGhribi/OpenStack-Juno-Installation/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /ChaimaGhribi/OpenStack-Juno-Installation/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">3</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/ChaimaGhribi/OpenStack-Juno-Installation/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /ChaimaGhribi/OpenStack-Juno-Installation/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

  <a href="/ChaimaGhribi/OpenStack-Juno-Installation/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /ChaimaGhribi/OpenStack-Juno-Installation/projects">
    <svg aria-hidden="true" class="octicon octicon-project" height="16" version="1.1" viewBox="0 0 15 16" width="15"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
    Projects
    <span class="counter">0</span>
</a>


  <a href="/ChaimaGhribi/OpenStack-Juno-Installation/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /ChaimaGhribi/OpenStack-Juno-Installation/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"/></svg>
    Pulse
</a>
  <a href="/ChaimaGhribi/OpenStack-Juno-Installation/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /ChaimaGhribi/OpenStack-Juno-Installation/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/ChaimaGhribi/OpenStack-Juno-Installation/blob/964c1ae450f6b1c9342b48514f427620a3941486/OpenStack-Juno-Installation.rst" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:7505989babd01b156a8f6e4315fd60b5 -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/ChaimaGhribi/OpenStack-Juno-Installation/blob/master/OpenStack-Juno-Installation.rst"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="BtnGroup float-right">
    <a href="/ChaimaGhribi/OpenStack-Juno-Installation/find/master"
          class="js-pjax-capture-input btn btn-sm BtnGroup-item"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/ChaimaGhribi/OpenStack-Juno-Installation"><span>OpenStack-Juno-Installation</span></a></span></span><span class="separator">/</span><strong class="final-path">OpenStack-Juno-Installation.rst</strong>
  </div>
</div>


  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/ChaimaGhribi/OpenStack-Juno-Installation/commit/bf789529443315cf47a68c8a673fbf5861ca13f2" data-pjax>
          bf78952
        </a>
        <relative-time datetime="2015-03-05T20:47:50Z">Mar 5, 2015</relative-time>
      </span>
      <div>
        <img alt="@MarouenMechtri" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/3438244?v=3&amp;s=40" width="20" />
        <a href="/MarouenMechtri" class="user-mention" rel="contributor">MarouenMechtri</a>
          <a href="/ChaimaGhribi/OpenStack-Juno-Installation/commit/bf789529443315cf47a68c8a673fbf5861ca13f2" class="message" data-pjax="true" title="Update OpenStack-Juno-Installation.rst">Update OpenStack-Juno-Installation.rst</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>2</strong>
         contributors
      </button>
          <a class="avatar-link tooltipped tooltipped-s" aria-label="MarouenMechtri" href="/ChaimaGhribi/OpenStack-Juno-Installation/commits/master/OpenStack-Juno-Installation.rst?author=MarouenMechtri"><img alt="@MarouenMechtri" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/3438244?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="ChaimaGhribi" href="/ChaimaGhribi/OpenStack-Juno-Installation/commits/master/OpenStack-Juno-Installation.rst?author=ChaimaGhribi"><img alt="@ChaimaGhribi" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/8246244?v=3&amp;s=40" width="20" /> </a>


    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@MarouenMechtri" height="24" src="https://avatars1.githubusercontent.com/u/3438244?v=3&amp;s=48" width="24" />
            <a href="/MarouenMechtri">MarouenMechtri</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ChaimaGhribi" height="24" src="https://avatars2.githubusercontent.com/u/8246244?v=3&amp;s=48" width="24" />
            <a href="/ChaimaGhribi">ChaimaGhribi</a>
          </li>
      </ul>
    </div>
  </div>


<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/ChaimaGhribi/OpenStack-Juno-Installation/raw/master/OpenStack-Juno-Installation.rst" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/ChaimaGhribi/OpenStack-Juno-Installation/blame/master/OpenStack-Juno-Installation.rst" class="btn btn-sm js-update-url-with-hash BtnGroup-item">Blame</a>
      <a href="/ChaimaGhribi/OpenStack-Juno-Installation/commits/master/OpenStack-Juno-Installation.rst" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>


        <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
        </button>
        <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
        </button>
  </div>

  <div class="file-info">
      1352 lines (849 sloc)
      <span class="file-info-divider"></span>
    34.3 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-openstack-juno-installation---multi-node" class="anchor" href="#openstack-juno-installation---multi-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>OpenStack Juno Installation - Multi Node</h1>
<p>Welcome to OpenStack Juno installation manual !</p>
<p>This document is based on <a href="http://docs.openstack.org/juno/install-guide/install/apt/content/index.html">the OpenStack Official Documentation</a> for Juno.</p>
<hr>
<p><strong>Contributors:</strong></p>
<p>Chaima Ghribi: <a href="mailto:chaima.ghribi@it-sudparis.eu">chaima.ghribi@it-sudparis.eu</a></p>
<p>Marouen Mechtri : <a href="mailto:marouen.mechtri@it-sudparis.eu">marouen.mechtri@it-sudparis.eu</a></p>
<p>Djamal Zeghlache : <a href="mailto:djamal.zeghlache@it-sudparis.eu">djamal.zeghlache@it-sudparis.eu</a></p>
<hr>
<div id="user-content-contents">
<p>Contents</p>
<ul>
<li><a href="#basic-architecture-and-network-configuration" id="user-content-id1">Basic Architecture and Network Configuration</a><ul>
<li><a href="#configure-controller-node" id="user-content-id2">Configure Controller node</a></li>
<li><a href="#configure-network-node" id="user-content-id3">Configure Network node</a></li>
<li><a href="#configure-compute-node" id="user-content-id4">Configure Compute node</a></li>
<li><a href="#verify-connectivity" id="user-content-id5">Verify connectivity</a></li>
</ul>
</li>
<li><a href="#install" id="user-content-id6">Install</a><ul>
<li><a href="#controller-node" id="user-content-id7">Controller Node</a><ul>
<li><a href="#install-the-supporting-services-ntp-mysql-and-rabbitmq" id="user-content-id8">Install the supporting services (NTP, MySQL and RabbitMQ)</a></li>
<li><a href="#install-the-identity-service-keystone" id="user-content-id9">Install the Identity Service (Keystone)</a></li>
<li><a href="#install-the-image-service-glance" id="user-content-id10">Install the image Service (Glance)</a></li>
<li><a href="#install-the-compute-service-nova" id="user-content-id11">Install the compute Service (Nova)</a></li>
<li><a href="#install-the-network-service-neutron" id="user-content-id12">Install the network Service (Neutron)</a></li>
<li><a href="#install-the-dashboard-service-horizon" id="user-content-id13">Install the dashboard Service (Horizon)</a></li>
</ul>
</li>
<li><a href="#network-node" id="user-content-id14">Network Node</a></li>
<li><a href="#compute-node" id="user-content-id15">Compute Node</a></li>
</ul>
</li>
<li><a href="#license" id="user-content-id16">License</a></li>
<li><a href="#authors" id="user-content-id17">Authors</a></li>
</ul>
</div>
<a name="user-content-basic-architecture-and-network-configuration"></a>
<h2><a id="user-content-basic-architecture-and-network-configuration" class="anchor" href="#basic-architecture-and-network-configuration" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id1">Basic Architecture and Network Configuration</a></h2>
<p>In this installation guide, we cover the step-by-step process of installing Openstack Juno on Ubuntu 14.04.  We consider a multi-node architecture with Openstack Networking (Neutron) that requires three node types:</p>
<ul>
<li><strong>Controller Node</strong> that runs management services (keystone, Horizon…) needed for OpenStack to function.</li>
<li><strong>Network Node</strong> that runs networking services and is responsible for virtual network provisioning  and for connecting virtual machines to external networks.</li>
<li><strong>Compute Node</strong> that runs the virtual machine instances in OpenStack.</li>
</ul>
<p>We have deployed a single compute node but you can simply add more compute nodes to our multi-node installation, if needed.</p>
<a href="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network-topo.jpg" target="_blank"><img alt="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network-topo.jpg" src="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network-topo.jpg" style="max-width:100%;"></a>
<p>For OpenStack Multi-Node setup you need to create three networks:</p>
<ul>
<li><strong>Management Network</strong> (10.0.0.0/24): A network segment used for administration, not accessible to the public Internet.</li>
<li><strong>VM Traffic Network</strong> (10.0.1.0/24): This network is used as internal network for traffic between virtual machines in OpenStack, and between the virtual machines and the network nodes that provide L3 routes out to the public network.</li>
<li><strong>Public Network</strong>: This network is connected to the controller node so users can access the OpenStack interfaces, and connected to the network node to provide VMs with publicly routable traffic functionality.</li>
</ul>
<p>In the next subsections, we describe in details how to set up, configure and test the network architecture. We want to make sure everything is ok before install ;)</p>
<p>So, let’s prepare the nodes for OpenStack installation!</p>
<a name="user-content-configure-controller-node"></a>
<h3><a id="user-content-configure-controller-node" class="anchor" href="#configure-controller-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id2">Configure Controller node</a></h3>
<p>The controller node has two Network Interfaces: eth0 (used for management network) and eth1 is external.</p>
<ul>
<li><p>Change to super user mode:</p>
<pre>sudo su
</pre>
</li>
<li><p>Set the hostname:</p>
<pre>vi /etc/hostname
controller
</pre>
</li>
<li><p>Edit /etc/hosts:</p>
<pre>vi /etc/hosts

#controller
10.0.0.11       controller

#network
10.0.0.21       network

# compute1
10.0.0.31       compute1
</pre>
</li>
<li><p>Note:</p>
<pre>Remove or comment the line beginning with 127.0.1.1.
</pre>
</li>
<li><p>Edit network settings to configure the interfaces eth0 and eth1:</p>
<pre>vi /etc/network/interfaces

# The management network interface
auto eth0
iface eth0 inet static
    address 10.0.0.11
    netmask 255.255.255.0
    network 10.0.0.0

# The public network interface
auto eth1
iface eth1 inet static
    address 192.168.100.11
    netmask 255.255.255.0
    network 192.168.100.0
    gateway 192.168.100.1
    dns-nameservers 8.8.8.8 8.8.4.4
</pre>
</li>
<li><p>Restart network and if needed <strong>reboot</strong> the system to activate the changes:</p>
<pre>ifdown eth0 &amp;&amp; ifup eth0

ifdown eth1 &amp;&amp; ifup eth1
</pre>
</li>
</ul>
<a name="user-content-configure-network-node"></a>
<h3><a id="user-content-configure-network-node" class="anchor" href="#configure-network-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id3">Configure Network node</a></h3>
<p>The network node has three network Interfaces: eth0 for management use: eth1
for connectivity between VMs and eth2 for external connectivity.</p>
<ul>
<li><p>Change to super user mode:</p>
<pre>sudo su
</pre>
</li>
<li><p>Set the hostname:</p>
<pre>vi /etc/hostname
network
</pre>
</li>
<li><p>Edit /etc/hosts:</p>
<pre>vi /etc/hosts

#network
10.0.0.21       network

#controller
10.0.0.11       controller

# compute1
10.0.0.31       compute1
</pre>
</li>
<li><p>Note:</p>
<pre>Remove or comment the line beginning with 127.0.1.1.
</pre>
</li>
<li><p>Edit network settings to configure the interfaces eth0, eth1 and eth2:</p>
<pre>vi /etc/network/interfaces

# The management network interface
auto eth0
iface eth0 inet static
    address 10.0.0.21
    netmask 255.255.255.0
    network 10.0.0.0


# VM traffic interface
auto eth1
iface eth1 inet static
    address 10.0.1.21
    netmask 255.255.255.0
    network 10.0.1.0

# The public network interface
auto eth2
iface eth2 inet static
    address 192.168.100.21
    netmask 255.255.255.0
    network 192.168.100.0
    gateway 192.168.100.1
    dns-nameservers 8.8.8.8 8.8.4.4
</pre>
</li>
<li><p>Restart network and if needed <strong>reboot</strong> the system to activate the changes:</p>
<pre>ifdown eth0 &amp;&amp; ifup eth0

ifdown eth1 &amp;&amp; ifup eth1

ifdown eth2 &amp;&amp; ifup eth2
</pre>
</li>
</ul>
<a name="user-content-configure-compute-node"></a>
<h3><a id="user-content-configure-compute-node" class="anchor" href="#configure-compute-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id4">Configure Compute node</a></h3>
<p>The network node has two network Interfaces: eth0 for management use and
eth1 for connectivity between VMs.</p>
<ul>
<li><p>Change to super user mode:</p>
<pre>sudo su
</pre>
</li>
<li><p>Set the hostname:</p>
<pre>vi /etc/hostname
compute1
</pre>
</li>
<li><p>Edit /etc/hosts:</p>
<pre>vi /etc/hosts

# compute1
10.0.0.31       compute1

#controller
10.0.0.11       controller

#network
10.0.0.21       network
</pre>
</li>
<li><p>Note:</p>
<pre>Remove or comment the line beginning with 127.0.1.1.
</pre>
</li>
<li><p>Edit network settings to configure the interfaces eth0 and eth1:</p>
<pre>vi /etc/network/interfaces

# The management network interface
auto eth0
iface eth0 inet static
    address 10.0.0.31
    netmask 255.255.255.0
    network 10.0.0.0

# VM traffic interface
auto eth1
iface eth1 inet static
    address 10.0.1.31
    netmask 255.255.255.0
    network 10.0.1.0
</pre>
</li>
<li><p>In order to be able to reach public network for installing openstack packages, we recommend to add a new interface (e.g. eth2) connected to the public network or configure nat Service on the management network.</p>
</li>
<li><p>Restart network and if needed <strong>reboot</strong> the system to activate the changes:</p>
<pre>ifdown eth0 &amp;&amp; ifup eth0

ifdown eth1 &amp;&amp; ifup eth1
</pre>
</li>
</ul>
<a name="user-content-verify-connectivity"></a>
<h3><a id="user-content-verify-connectivity" class="anchor" href="#verify-connectivity" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id5">Verify connectivity</a></h3>
<p>We recommend that you verify network connectivity to the internet and among the nodes before proceeding further.</p>
<ul>
<li><p>From the controller node:</p>
<pre># ping a site on the internet:
ping openstack.org

# ping the management interface on the network node:
ping network

# ping the management interface on the compute node:
ping compute1
</pre>
</li>
<li><p>From the network node:</p>
<pre># ping a site on the internet:
ping openstack.org

# ping the management interface on the controller node:
ping controller

# ping the VM traffic interface on the compute node:
ping 10.0.1.31
</pre>
</li>
<li><p>From the compute node:</p>
<pre># ping a site on the internet:
ping openstack.org

# ping the management interface on the controller node:
ping controller

# ping the VM traffic interface on the network node:
ping 10.0.1.21
</pre>
</li>
</ul>
<a name="user-content-install"></a>
<h2><a id="user-content-install" class="anchor" href="#install" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id6">Install</a></h2>
<p>Now everything is ok :) So let's go ahead and install it !</p>
<a name="user-content-controller-node"></a>
<h3><a id="user-content-controller-node" class="anchor" href="#controller-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id7">Controller Node</a></h3>
<p>Let's start with the controller ! the cornerstone !</p>
<p>Here we've installed the basic services (keystone, glance, nova,neutron and horizon) and also the supporting services
such as MySql database, message broker (RabbitMQ), and NTP.</p>
<p>Additional installation guides for optional services (Heat, Ceilometer...) are also provided
<a href="https://github.com/MarouenMechtri/Heat-Installation-for-OpenStack-Juno">Heat installation guide</a>,
<a href="https://github.com/MarouenMechtri/Ceilometer-Installation-for-OpenStack-Juno">Ceilometer installation guide</a>.</p>
<a href="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/controller.jpg" target="_blank"><img alt="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/controller.jpg" src="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/controller.jpg" style="max-width:100%;"></a>
<a name="user-content-install-the-supporting-services-ntp-mysql-and-rabbitmq"></a>
<h4><a id="user-content-install-the-supporting-services-ntp-mysql-and-rabbitmq" class="anchor" href="#install-the-supporting-services-ntp-mysql-and-rabbitmq" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id8">Install the supporting services (NTP, MySQL and RabbitMQ)</a></h4>
<ul>
<li><p>Install NTP (Network Time Protocol) service:</p>
<pre>apt-get install -y ntp
</pre>
</li>
<li><p>Edit the /etc/ntp.conf file:</p>
<pre>server 0.ubuntu.pool.ntp.org iburst
server 1.ubuntu.pool.ntp.org iburst
server 2.ubuntu.pool.ntp.org iburst
server 3.ubuntu.pool.ntp.org iburst

# Use Ubuntu's ntp server as a fallback.
server ntp.ubuntu.com iburst

restrict -4 default kod notrap nomodify
restrict -6 default kod notrap nomodify
</pre>
</li>
<li><p>Restart the NTP service:</p>
<pre>service ntp restart
</pre>
</li>
<li><p>Enable the OpenStack repository:</p>
<pre>apt-get install -y ubuntu-cloud-keyring
echo "deb http://ubuntu-cloud.archive.canonical.com/ubuntu" \
"trusty-updates/juno main" &gt; /etc/apt/sources.list.d/cloudarchive-juno.list
</pre>
</li>
<li><p>Upgrade the packages on your system:</p>
<pre>apt-get update -y &amp;&amp; apt-get dist-upgrade -y
</pre>
</li>
<li><p>Install MySQL:</p>
<pre>apt-get install -y mariadb-server python-mysqldb
</pre>
</li>
<li><p>Edit /etc/mysql/my.cnf file:</p>
<pre>vi /etc/mysql/my.cnf
[mysqld]
bind-address = 10.0.0.11
default-storage-engine = innodb
innodb_file_per_table
collation-server = utf8_general_ci
init-connect = 'SET NAMES utf8'
character-set-server = utf8
</pre>
</li>
<li><p>Restart the MySQL service:</p>
<pre>service mysql restart
</pre>
</li>
<li><p>Secure the database service:</p>
<pre>mysql_secure_installation
</pre>
</li>
<li><p>Install RabbitMQ (Message Queue):</p>
<pre>apt-get install -y rabbitmq-server
</pre>
</li>
<li><p>Change the password:</p>
<pre>rabbitmqctl change_password guest service_pass
</pre>
</li>
</ul>
<a name="user-content-install-the-identity-service-keystone"></a>
<h4><a id="user-content-install-the-identity-service-keystone" class="anchor" href="#install-the-identity-service-keystone" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id9">Install the Identity Service (Keystone)</a></h4>
<ul>
<li><p>Create a MySQL database for keystone:</p>
<pre>mysql -u root -p

CREATE DATABASE keystone;
GRANT ALL PRIVILEGES ON keystone.* TO 'keystone'@'localhost' IDENTIFIED BY 'KEYSTONE_DBPASS';
GRANT ALL PRIVILEGES ON keystone.* TO 'keystone'@'%' IDENTIFIED BY 'KEYSTONE_DBPASS';

exit;
</pre>
</li>
<li><p>Install keystone packages:</p>
<pre>apt-get install -y keystone python-keystoneclient
</pre>
</li>
<li><p>Remove Keystone SQLite database:</p>
<pre>rm -f /var/lib/keystone/keystone.db
</pre>
</li>
<li><p>Edit /etc/keystone/keystone.conf:</p>
<pre> vi /etc/keystone/keystone.conf

[database]
replace connection = sqlite:////var/lib/keystone/keystone.db by
connection = mysql://keystone:KEYSTONE_DBPASS@controller/keystone

[DEFAULT]
admin_token = ADMIN
verbose = True

[token]
provider = keystone.token.providers.uuid.Provider
driver = keystone.token.persistence.backends.sql.Token

[revoke]
driver = keystone.contrib.revoke.backends.sql.Revoke
</pre>
</li>
<li><p>Populate the Identity service database:</p>
<pre>su -s /bin/sh -c "keystone-manage db_sync" keystone
</pre>
</li>
<li><p>Restart the Identity service:</p>
<pre>service keystone restart
</pre>
</li>
<li><p>We recommend that you use cron to configure a periodic task that purges expired tokens hourly:</p>
<pre>(crontab -l -u keystone 2&gt;&amp;1 | grep -q token_flush) || \
echo '@hourly /usr/bin/keystone-manage token_flush &gt;/var/log/keystone/keystone-tokenflush.log 2&gt;&amp;1' \
&gt;&gt; /var/spool/cron/crontabs/keystone
</pre>
</li>
<li><p>Check synchronization:</p>
<pre>mysql -u root -p keystone
show TABLES;
</pre>
</li>
<li><p>Define users, tenants, and roles:</p>
<pre>export OS_SERVICE_TOKEN=ADMIN
export OS_SERVICE_ENDPOINT=http://controller:35357/v2.0

#Create an administrative user
keystone tenant-create --name admin --description "Admin Tenant"
keystone user-create --name admin --pass admin_pass --email admin@domain.com
keystone role-create --name admin
keystone user-role-add --user admin --tenant admin --role admin


#Create a normal user
keystone tenant-create --name demo --description "Demo Tenant"
keystone user-create --name demo --tenant demo --pass demo_pass --email demo@domain.com


#Create a service tenant
keystone tenant-create --name service --description "Service Tenant"
</pre>
</li>
<li><p>Define services and API endpoints:</p>
<pre>keystone service-create --name keystone --type identity --description "OpenStack Identity"

keystone endpoint-create \
--service-id $(keystone service-list | awk '/ identity / {print $2}') \
--publicurl http://controller:5000/v2.0 \
--internalurl http://controller:5000/v2.0 \
--adminurl http://controller:35357/v2.0 \
--region regionOne
</pre>
</li>
<li><p>Test Keystone:</p>
<pre>#clear the values in the OS_SERVICE_TOKEN and OS_SERVICE_ENDPOINT environment variables:
unset OS_SERVICE_TOKEN OS_SERVICE_ENDPOINT

#Request an authentication token:
keystone --os-tenant-name admin --os-username admin --os-password admin_pass \
--os-auth-url http://controller:35357/v2.0 token-get

#List tenants:
keystone --os-tenant-name admin --os-username admin --os-password admin_pass \
--os-auth-url http://controller:35357/v2.0 tenant-list

#List users:
keystone --os-tenant-name admin --os-username admin --os-password admin_pass \
--os-auth-url http://controller:35357/v2.0 user-list

#List roles:
keystone --os-tenant-name admin --os-username admin --os-password admin_pass \
--os-auth-url http://controller:35357/v2.0 role-list

#Request an authentication token:
keystone --os-tenant-name demo --os-username demo --os-password demo_pass \
--os-auth-url http://controller:35357/v2.0 token-get

#Attempt to list users to verify that demo tenant cannot list users:
keystone --os-tenant-name demo --os-username demo --os-password demo_pass \
--os-auth-url http://controller:35357/v2.0 user-list
You are not authorized to perform the requested action: admin_required (HTTP 403)
</pre>
</li>
<li><p>Create a simple credential file:</p>
<pre>vi admin_creds
#Paste the following:
export OS_TENANT_NAME=admin
export OS_USERNAME=admin
export OS_PASSWORD=admin_pass
export OS_AUTH_URL=http://controller:35357/v2.0

vi demo_creds
#Paste the following:
export OS_TENANT_NAME=demo
export OS_USERNAME=demo
export OS_PASSWORD=demo_pass
export OS_AUTH_URL=http://controller:5000/v2.0
</pre>
</li>
<li><p>To load client environment scripts:</p>
<pre>source admin_creds
</pre>
</li>
</ul>
<a name="user-content-install-the-image-service-glance"></a>
<h4><a id="user-content-install-the-image-service-glance" class="anchor" href="#install-the-image-service-glance" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id10">Install the image Service (Glance)</a></h4>
<ul>
<li><p>Create a MySQL database for Glance:</p>
<pre>mysql -u root -p

CREATE DATABASE glance;
GRANT ALL PRIVILEGES ON glance.* TO 'glance'@'localhost' IDENTIFIED BY 'GLANCE_DBPASS';
GRANT ALL PRIVILEGES ON glance.* TO 'glance'@'%' IDENTIFIED BY 'GLANCE_DBPASS';

exit;
</pre>
</li>
<li><p>Configure service user and role:</p>
<pre>source admin_creds

keystone user-create --name glance --pass service_pass
keystone user-role-add --user glance --tenant service --role admin
</pre>
</li>
<li><p>Register the service and create the endpoint:</p>
<pre>keystone service-create --name glance --type image --description "OpenStack Image Service"
keystone endpoint-create \
--service-id $(keystone service-list | awk '/ image / {print $2}') \
--publicurl http://controller:9292 \
--internalurl http://controller:9292 \
--adminurl http://controller:9292 \
--region regionOne
</pre>
</li>
<li><p>Install Glance packages:</p>
<pre>apt-get install -y glance python-glanceclient
</pre>
</li>
<li><p>Update /etc/glance/glance-api.conf:</p>
<pre>vi /etc/glance/glance-api.conf

[database]
replace sqlite_db = /var/lib/glance/glance.sqlite with
connection = mysql://glance:GLANCE_DBPASS@controller/glance

[DEFAULT]
notification_driver = noop
verbose = True

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = glance
admin_password = service_pass

[paste_deploy]
flavor = keystone

[glance_store]
default_store = file
filesystem_store_datadir = /var/lib/glance/images/
</pre>
</li>
<li><p>Update /etc/glance/glance-registry.conf:</p>
<pre>vi /etc/glance/glance-registry.conf

[database]
replace sqlite_db = /var/lib/glance/glance.sqlite with:
connection = mysql://glance:GLANCE_DBPASS@controller/glance

[DEFAULT]
notification_driver = noop
verbose = True

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = glance
admin_password = service_pass


[paste_deploy]
flavor = keystone
</pre>
</li>
<li><p>Populate the Image Service database:</p>
<pre>su -s /bin/sh -c "glance-manage db_sync" glance
</pre>
</li>
<li><p>Restart the Image Service services:</p>
<pre>service glance-registry restart
service glance-api restart
</pre>
</li>
<li><p>Test Glance, upload the cirros cloud image:</p>
<pre>source admin_creds
mkdir /tmp/images

wget -P /tmp/images http://cdn.download.cirros-cloud.net/0.3.3/cirros-0.3.3-x86_64-disk.img

glance image-create --name "cirros-0.3.3-x86_64" --file /tmp/images/cirros-0.3.3-x86_64-disk.img \
--disk-format qcow2 --container-format bare --is-public True --progress

rm -r /tmp/images
</pre>
</li>
<li><p>List Images:</p>
<pre>glance image-list
</pre>
</li>
</ul>
<a name="user-content-install-the-compute-service-nova"></a>
<h4><a id="user-content-install-the-compute-service-nova" class="anchor" href="#install-the-compute-service-nova" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id11">Install the compute Service (Nova)</a></h4>
<ul>
<li><p>Create a Mysql database for Nova:</p>
<pre>mysql -u root -p

CREATE DATABASE nova;
GRANT ALL PRIVILEGES ON nova.* TO 'nova'@'localhost' IDENTIFIED BY 'NOVA_DBPASS';
GRANT ALL PRIVILEGES ON nova.* TO 'nova'@'%' IDENTIFIED BY 'NOVA_DBPASS';

exit;
</pre>
</li>
<li><p>Configure service user and role:</p>
<pre>source admin_creds
keystone user-create --name nova --pass service_pass
keystone user-role-add --user nova --tenant service --role admin
</pre>
</li>
<li><p>Register the service and create the endpoint:</p>
<pre>keystone service-create --name nova --type compute --description "OpenStack Compute"
keystone endpoint-create \
--service-id $(keystone service-list | awk '/ compute / {print $2}') \
--publicurl http://controller:8774/v2/%\(tenant_id\)s \
--internalurl http://controller:8774/v2/%\(tenant_id\)s \
--adminurl http://controller:8774/v2/%\(tenant_id\)s \
--region regionOne
</pre>
</li>
<li><p>Install nova packages:</p>
<pre>apt-get install -y nova-api nova-cert nova-conductor nova-consoleauth \
nova-novncproxy nova-scheduler python-novaclient
</pre>
</li>
<li><p>Edit the /etc/nova/nova.conf:</p>
<pre>vi /etc/nova/nova.conf

[database]
connection = mysql://nova:NOVA_DBPASS@controller/nova

[DEFAULT]
rpc_backend = rabbit
rabbit_host = controller
rabbit_password = service_pass
auth_strategy = keystone
my_ip = 10.0.0.11
vncserver_listen = 10.0.0.11
vncserver_proxyclient_address = 10.0.0.11
verbose = True


[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = nova
admin_password = service_pass

[glance]
host = controller
</pre>
</li>
<li><p>Populate the Compute database:</p>
<pre>su -s /bin/sh -c "nova-manage db sync" nova
</pre>
</li>
<li><p>Restart nova-* services:</p>
<pre>service nova-api restart
service nova-cert restart
service nova-consoleauth restart
service nova-scheduler restart
service nova-conductor restart
service nova-novncproxy restart
</pre>
</li>
<li><p>Remove the SQLite database file:</p>
<pre>rm -f /var/lib/nova/nova.sqlite
</pre>
</li>
<li><p>Check Nova is running</p>
<pre>source admin_creds
nova service-list
</pre>
</li>
<li><p>To verify your configuration, list available images:</p>
<pre>source admin_creds
nova image-list
</pre>
</li>
</ul>
<a name="user-content-install-the-network-service-neutron"></a>
<h4><a id="user-content-install-the-network-service-neutron" class="anchor" href="#install-the-network-service-neutron" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id12">Install the network Service (Neutron)</a></h4>
<ul>
<li><p>Create a MySql database for Neutron:</p>
<pre>mysql -u root -p

CREATE DATABASE neutron;
GRANT ALL PRIVILEGES ON neutron.* TO neutron@'localhost' IDENTIFIED BY 'NEUTRON_DBPASS';
GRANT ALL PRIVILEGES ON neutron.* TO neutron@'%' IDENTIFIED BY 'NEUTRON_DBPASS';

exit;
</pre>
</li>
<li><p>Configure service user and role:</p>
<pre>source admin_creds
keystone user-create --name neutron --pass service_pass
keystone user-role-add --user neutron --tenant service --role admin
</pre>
</li>
<li><p>Register the service and create the endpoint:</p>
<pre>keystone service-create --name neutron --type network --description "OpenStack Networking"

keystone endpoint-create \
--service-id $(keystone service-list | awk '/ network / {print $2}') \
--publicurl http://controller:9696 \
--adminurl http://controller:9696 \
--internalurl http://controller:9696 \
--region regionOne
</pre>
</li>
<li><p>Install the Networking components:</p>
<pre>apt-get install -y neutron-server neutron-plugin-ml2 python-neutronclient
</pre>
</li>
<li><p>Update /etc/neutron/neutron.conf:</p>
<pre>vi /etc/neutron/neutron.conf

[database]
replace connection = sqlite:////var/lib/neutron/neutron.sqlite with
connection = mysql://neutron:NEUTRON_DBPASS@controller/neutron

[DEFAULT]
rpc_backend = rabbit
rabbit_host = controller
rabbit_password = service_pass

auth_strategy = keystone

core_plugin = ml2
service_plugins = router
allow_overlapping_ips = True

notify_nova_on_port_status_changes = True
notify_nova_on_port_data_changes = True
nova_url = http://controller:8774/v2
nova_admin_auth_url = http://controller:35357/v2.0
nova_region_name = regionOne
nova_admin_username = nova
# Replace the SERVICE_TENANT_ID with the output of this command
# (keystone tenant-list | awk '/ service / { print $2 }')
nova_admin_tenant_id = SERVICE_TENANT_ID
nova_admin_password = service_pass

verbose = True

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = neutron
admin_password = service_pass
</pre>
</li>
<li><p>Configure the Modular Layer 2 (ML2) plug-in:</p>
<pre>vi /etc/neutron/plugins/ml2/ml2_conf.ini

[ml2]
type_drivers = flat,gre
tenant_network_types = gre
mechanism_drivers = openvswitch

[ml2_type_gre]
tunnel_id_ranges = 1:1000

[securitygroup]
enable_security_group = True
enable_ipset = True
firewall_driver = neutron.agent.linux.iptables_firewall.OVSHybridIptablesFirewallDriver
</pre>
</li>
<li><p>Configure Compute to use Networking:</p>
<pre>add in /etc/nova/nova.conf

vi /etc/nova/nova.conf

[DEFAULT]
network_api_class = nova.network.neutronv2.api.API
security_group_api = neutron
linuxnet_interface_driver = nova.network.linux_net.LinuxOVSInterfaceDriver
firewall_driver = nova.virt.firewall.NoopFirewallDriver

[neutron]
url = http://controller:9696
auth_strategy = keystone
admin_auth_url = http://controller:35357/v2.0
admin_tenant_name = service
admin_username = neutron
admin_password = service_pass
</pre>
</li>
<li><p>Populate the database:</p>
<pre>su -s /bin/sh -c "neutron-db-manage --config-file /etc/neutron/neutron.conf \
--config-file /etc/neutron/plugins/ml2/ml2_conf.ini upgrade juno" neutron
</pre>
</li>
<li><p>Restart the Compute services:</p>
<pre>service nova-api restart
service nova-scheduler restart
service nova-conductor restart
</pre>
</li>
<li><p>Restart the Networking service:</p>
<pre>service neutron-server restart
</pre>
</li>
</ul>
<a name="user-content-install-the-dashboard-service-horizon"></a>
<h4><a id="user-content-install-the-dashboard-service-horizon" class="anchor" href="#install-the-dashboard-service-horizon" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id13">Install the dashboard Service (Horizon)</a></h4>
<ul>
<li><p>Install the required packages:</p>
<pre>apt-get install -y openstack-dashboard apache2 libapache2-mod-wsgi memcached python-memcache
</pre>
</li>
<li><p>You can remove the openstack-dashboard-ubuntu-theme package:</p>
<pre>apt-get remove -y --purge openstack-dashboard-ubuntu-theme
</pre>
</li>
<li><p>Edit /etc/openstack-dashboard/local_settings.py:</p>
<pre>vi /etc/openstack-dashboard/local_settings.py

OPENSTACK_HOST = "controller"
ALLOWED_HOSTS = ['*']

CACHES = {
           'default': { 'BACKEND': 'django.core.cache.backends.memcached.
                         MemcachedCache', 'LOCATION': '127.0.0.1:11211',
                      }
}
</pre>
</li>
<li><p>Restart the web server and session storage service:</p>
<pre>service apache2 restart
service memcached restart
</pre>
</li>
<li><p>Check OpenStack Dashboard at <a href="http://controller/horizon">http://controller/horizon</a>  login admin/admin_pass</p>
</li>
</ul>
<a name="user-content-network-node"></a>
<h3><a id="user-content-network-node" class="anchor" href="#network-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id14">Network Node</a></h3>
<p>Now, let's move to second step!</p>
<p>The network node runs the Networking plug-in and different agents (see the Figure below).</p>
<a href="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network.jpg" target="_blank"><img alt="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network.jpg" src="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/network.jpg" style="max-width:100%;"></a>
<ul>
<li><p>Install NTP service:</p>
<pre>apt-get install -y ntp
</pre>
</li>
<li><p>Edit the /etc/ntp.conf file:</p>
<pre>vi /etc/ntp.conf

[replace]
server 0.ubuntu.pool.ntp.org
server 1.ubuntu.pool.ntp.org
server 2.ubuntu.pool.ntp.org
server 3.ubuntu.pool.ntp.org

# Use Ubuntu's ntp server as a fallback.
server ntp.ubuntu.com

[with]
server controller iburst
</pre>
</li>
<li><p>Restart NTP service:</p>
<pre>service ntp restart
</pre>
</li>
<li><p>Enable the OpenStack repository:</p>
<pre>apt-get install -y ubuntu-cloud-keyring
echo "deb http://ubuntu-cloud.archive.canonical.com/ubuntu" \
"trusty-updates/juno main" &gt; /etc/apt/sources.list.d/cloudarchive-juno.list
</pre>
</li>
<li><p>Upgrade the packages on your system:</p>
<pre>apt-get update -y &amp;&amp; apt-get dist-upgrade -y
</pre>
</li>
<li><p>Edit /etc/sysctl.conf to contain the following:</p>
<pre>vi /etc/sysctl.conf
net.ipv4.ip_forward=1
net.ipv4.conf.all.rp_filter=0
net.ipv4.conf.default.rp_filter=0
</pre>
</li>
<li><p>Implement the changes:</p>
<pre>sysctl -p
</pre>
</li>
<li><p>Install the Networking components:</p>
<pre>apt-get install -y neutron-plugin-ml2 neutron-plugin-openvswitch-agent \
neutron-l3-agent neutron-dhcp-agent
</pre>
</li>
<li><p>Update /etc/neutron/neutron.conf:</p>
<pre>vi /etc/neutron/neutron.conf

[DEFAULT]
rpc_backend = rabbit
rabbit_host = controller
rabbit_password = service_pass

auth_strategy = keystone

core_plugin = ml2
service_plugins = router
allow_overlapping_ips = True

verbose = True

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = neutron
admin_password = service_pass

**[comment out this line]**
connection = sqlite:////var/lib/neutron/neutron.sqlite
</pre>
</li>
<li><p>Edit the /etc/neutron/plugins/ml2/ml2_conf.ini:</p>
<pre>vi /etc/neutron/plugins/ml2/ml2_conf.ini

[ml2]
type_drivers = flat,gre
tenant_network_types = gre
mechanism_drivers = openvswitch

[ml2_type_flat]
flat_networks = external

[ml2_type_gre]
tunnel_id_ranges = 1:1000

[securitygroup]
enable_security_group = True
enable_ipset = True
firewall_driver = neutron.agent.linux.iptables_firewall.OVSHybridIptablesFirewallDriver

[ovs]
local_ip = 10.0.1.21
enable_tunneling = True
bridge_mappings = external:br-ex

[agent]
tunnel_types = gre
</pre>
</li>
<li><p>Edit the /etc/neutron/l3_agent.ini:</p>
<pre>vi /etc/neutron/l3_agent.ini

[DEFAULT]
interface_driver = neutron.agent.linux.interface.OVSInterfaceDriver
use_namespaces = True
external_network_bridge = br-ex
router_delete_namespaces = True

verbose = True
</pre>
</li>
<li><p>Edit the /etc/neutron/dhcp_agent.ini:</p>
<pre>vi /etc/neutron/dhcp_agent.ini

[DEFAULT]
interface_driver = neutron.agent.linux.interface.OVSInterfaceDriver
dhcp_driver = neutron.agent.linux.dhcp.Dnsmasq
use_namespaces = True
dhcp_delete_namespaces = True

verbose = True

dnsmasq_config_file = /etc/neutron/dnsmasq-neutron.conf
</pre>
</li>
<li><p>Edit the /etc/neutron/dnsmasq-neutron.conf file:</p>
<pre>vi /etc/neutron/dnsmasq-neutron.conf

dhcp-option-force=26,1454
</pre>
</li>
<li><p>Kill any existing dnsmasq processes:</p>
<pre>pkill dnsmasq
</pre>
</li>
<li><p>Edit the /etc/neutron/metadata_agent.ini:</p>
<pre>vi /etc/neutron/metadata_agent.ini

[DEFAULT]
auth_url = http://controller:5000/v2.0
auth_region = regionOne
admin_tenant_name = service
admin_user = neutron
admin_password = service_pass

nova_metadata_ip = controller

metadata_proxy_shared_secret = METADATA_SECRET

verbose = True
</pre>
</li>
<li><p>Note: On the <strong>controller node</strong>, edit the /etc/nova/nova.conf file:</p>
<pre>vi /etc/nova/nova.conf

[DEFAULT]
service_metadata_proxy = True
metadata_proxy_shared_secret = METADATA_SECRET
</pre>
</li>
<li><p>Note: On the <strong>controller node</strong>, restart nova-api service:</p>
<pre>service nova-api restart
</pre>
</li>
<li><p>Restart openVSwitch:</p>
<pre>service openvswitch-switch restart
</pre>
</li>
<li><p>Add the external bridge:</p>
<pre>ovs-vsctl add-br br-ex
</pre>
</li>
<li><p>Add the eth2 to the br-ex:</p>
<pre>ovs-vsctl add-port br-ex eth2
</pre>
</li>
<li><p>Edit /etc/network/interfaces:</p>
<pre>vi /etc/network/interfaces

# The public network interface
auto eth2
iface eth2 inet manual
    up ip link set dev $IFACE up
    down ip link set dev $IFACE down

auto br-ex
iface br-ex inet static
    address 192.168.100.21
    netmask 255.255.255.0
    network 192.168.100.0
    gateway 192.168.100.1
    dns-nameservers 8.8.8.8 8.8.4.4
</pre>
</li>
<li><p>Restart network:</p>
<pre>ifdown eth2 &amp;&amp; ifup eth2

ifdown br-ex &amp;&amp; ifup br-ex
</pre>
</li>
<li><p>Restart the Networking services:</p>
<pre>service neutron-plugin-openvswitch-agent restart
service neutron-l3-agent restart
service neutron-dhcp-agent restart
service neutron-metadata-agent restart
</pre>
</li>
<li><p>On the <strong>controller node</strong>, perform these commands to check Neutron agents:</p>
<pre>source admin_creds
neutron agent-list
</pre>
</li>
</ul>
<a name="user-content-compute-node"></a>
<h3><a id="user-content-compute-node" class="anchor" href="#compute-node" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id15">Compute Node</a></h3>
<p>Finally, let's install the services on the compute node!</p>
<p>It uses KVM as hypervisor and runs nova-compute, the Networking plug-in and layer 2 agent.</p>
<a href="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/compute.jpg" target="_blank"><img alt="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/compute.jpg" src="https://raw.githubusercontent.com/ChaimaGhribi/OpenStack-Juno-Installation/master/images/compute.jpg" style="max-width:100%;"></a>
<ul>
<li><p>Install ntp service:</p>
<pre>apt-get install -y ntp
</pre>
</li>
<li><p>Set the compute node to follow up your conroller node:</p>
<pre>vi /etc/ntp.conf

[replace]
server 0.ubuntu.pool.ntp.org
server 1.ubuntu.pool.ntp.org
server 2.ubuntu.pool.ntp.org
server 3.ubuntu.pool.ntp.org

# Use Ubuntu's ntp server as a fallback.
server ntp.ubuntu.com

[with]
server controller iburst
</pre>
</li>
<li><p>Restart NTP service:</p>
<pre>service ntp restart
</pre>
</li>
<li><p>Enable the OpenStack repository:</p>
<pre>apt-get install -y ubuntu-cloud-keyring
echo "deb http://ubuntu-cloud.archive.canonical.com/ubuntu" \
"trusty-updates/juno main" &gt; /etc/apt/sources.list.d/cloudarchive-juno.list
</pre>
</li>
<li><p>Upgrade the packages on your system:</p>
<pre>apt-get update -y &amp;&amp; apt-get dist-upgrade -y
</pre>
</li>
<li><p>Install the Compute packages:</p>
<pre>apt-get install -y nova-compute sysfsutils
</pre>
</li>
<li><p>Modify the /etc/nova/nova.conf like this:</p>
<pre>vi /etc/nova/nova.conf
[DEFAULT]
verbose = True

auth_strategy = keystone

rpc_backend = rabbit
rabbit_host = controller
rabbit_password = service_pass

my_ip = 10.0.0.31

vnc_enabled = True
vncserver_listen = 0.0.0.0
vncserver_proxyclient_address = 10.0.0.31
novncproxy_base_url = http://192.168.100.11:6080/vnc_auto.html

network_api_class = nova.network.neutronv2.api.API
security_group_api = neutron
linuxnet_interface_driver = nova.network.linux_net.LinuxOVSInterfaceDriver
firewall_driver = nova.virt.firewall.NoopFirewallDriver

vif_plugging_is_fatal=false
vif_plugging_timeout=0

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = nova
admin_password = service_pass

[glance]
host = controller

[neutron]
url = http://controller:9696
auth_strategy = keystone
admin_auth_url = http://controller:35357/v2.0
admin_tenant_name = service
admin_username = neutron
admin_password = service_pass
</pre>
</li>
<li><p>Edit /etc/nova/nova-compute.conf with the correct hypervisor type (set to qemu if using virtualbox for example, kvm is default):</p>
<pre>vi /etc/nova/nova-compute.conf

[DEFAULT]
compute_driver=libvirt.LibvirtDriver

[libvirt]
virt_type=qemu
</pre>
</li>
<li><p>Delete /var/lib/nova/nova.sqlite file:</p>
<pre>rm -f /var/lib/nova/nova.sqlite
</pre>
</li>
<li><p>Edit /etc/sysctl.conf to contain the following:</p>
<pre>vi /etc/sysctl.conf
net.ipv4.conf.all.rp_filter=0
net.ipv4.conf.default.rp_filter=0
</pre>
</li>
<li><p>Implement the changes:</p>
<pre>sysctl -p
</pre>
</li>
<li><p>Install the Networking components:</p>
<pre>apt-get install -y neutron-plugin-ml2 neutron-plugin-openvswitch-agent
</pre>
</li>
<li><p>Update /etc/neutron/neutron.conf:</p>
<pre>vi /etc/neutron/neutron.conf

[DEFAULT]
verbose = True

rpc_backend = rabbit
rabbit_host = controller
rabbit_password = service_pass

auth_strategy = keystone

core_plugin = ml2
service_plugins = router
allow_overlapping_ips = True

[keystone_authtoken]
auth_uri = http://controller:5000/v2.0
identity_uri = http://controller:35357
admin_tenant_name = service
admin_user = neutron
admin_password = service_pass

**[remove]**
connection = sqlite:////var/lib/neutron/neutron.sqlite
</pre>
</li>
<li><p>Configure the Modular Layer 2 (ML2) plug-in:</p>
<pre>vi /etc/neutron/plugins/ml2/ml2_conf.ini

[ml2]
type_drivers = flat,gre
tenant_network_types = gre
mechanism_drivers = openvswitch

[ml2_type_gre]
tunnel_id_ranges = 1:1000

[securitygroup]
enable_security_group = True
enable_ipset = True
firewall_driver = neutron.agent.linux.iptables_firewall.OVSHybridIptablesFirewallDriver

[ovs]
local_ip = 10.0.1.31
enable_tunneling = True

[agent]
tunnel_types = gre
</pre>
</li>
<li><p>Restart the OVS service:</p>
<pre>service openvswitch-switch restart
</pre>
</li>
<li><p>Restart nova-compute services:</p>
<pre>service nova-compute restart
</pre>
</li>
<li><p>Restart the Open vSwitch (OVS) agent:</p>
<pre>service neutron-plugin-openvswitch-agent restart
</pre>
</li>
<li><p>On the <strong>controller node</strong>, list agents to verify successful launch of the neutron agents:</p>
<pre>source admin_creds
neutron agent-list
nova service-list
</pre>
</li>
</ul>
<p>That's it !! ;) Just try it!</p>
<p>If you want to create your first instance with Neutron, follow the instructions in our VM creation guide available
here <a href="https://github.com/ChaimaGhribi/OpenStack-Juno-Installation/blob/master/Create-your-first-instance-with-Neutron.rst">Create-First-Instance-with-Neutron</a>.</p>
<p>Your contributions are welcome, as are questions and requests for help :)</p>
<p>Hope this manual will be helpful and simple!</p>
<a name="user-content-license"></a>
<h2><a id="user-content-license" class="anchor" href="#license" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id16">License</a></h2>
<p>Institut Mines Télécom - Télécom SudParis</p>
<p>Copyright (C) 2015  Authors</p>
<p>Original Authors - Chaima Ghribi and Marouen Mechtri</p>
<p>Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except</p>
<p>in compliance with the License. You may obtain a copy of the License at:</p>
<pre>http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
</pre>
<a name="user-content-authors"></a>
<h2><a id="user-content-authors" class="anchor" href="#authors" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="#id17">Authors</a></h2>
<p>Copyright (C) <a href="https://www.linkedin.com/pub/chaima-ghribi/15/b78/997/">Chaima Ghribi</a> : <a href="mailto:chaima.ghribi@it-sudparis.eu">chaima.ghribi@it-sudparis.eu</a></p>
<p>Copyright (C) <a href="https://www.linkedin.com/in/mechtri">Marouen Mechtri</a> : <a href="mailto:marouen.mechtri@it-sudparis.eu">marouen.mechtri@it-sudparis.eu</a></p>

</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.05161s from github-fe-9d6fe79.cp1-iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
      </button>
      You can't perform that action at this time.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/compat-30ce4c86c27f88c3d1b4eb03efda59b45d8d7c871880dee0b8f73d5ef1b25fdf.js"></script>
      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-05c8a25698c5f34cfcd4d6d32b90bea58249cb4011dfbd7aa7d8942aa8948ba0.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-ba2f1ce9bf0ac7ac724cbd7a665e01962357b733322d682c710a802226e445a1.js"></script>
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
    </button>
  </div>
</div>

  </body>
</html>

