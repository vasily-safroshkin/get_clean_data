



<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>coursera-getting-cleaning-data/CodeBook.md at master · vasily_safroshkin/get_clean_data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="vasily_safroshkin/get_clean_data" name="twitter:title" /><meta content="coursera-getting-cleaning-data - Repository for Getting and Cleaning Data Course Project " name="twitter:description" /><meta content="https://avatars1.githubusercontent.com/u/38604?v=3&amp;s=400" name="twitter:image:src" />
<meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars1.githubusercontent.com/u/38604?v=3&amp;s=400" property="og:image" /><meta content="vasily_safroshkin/get_clean_data" property="og:title" /><meta content="https://github.com/vasily_safroshkin/get_clean_data" property="og:url" /><meta content="coursera-getting-cleaning-data - Repository for Getting and Cleaning Data Course Project " property="og:description" />

      <meta name="browser-stats-url" content="/_stats">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="conduit-xhr" href="https://ghconduit.com:25035">
    <link rel="xhr-socket" href="/_sockets">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="53DCA153:18A7:10DBBF8:5495943D" name="octolytics-dimension-request_id" /><meta content="9738662" name="octolytics-actor-id" /><meta content="vasily-safroshkin" name="octolytics-actor-login" /><meta content="7c07b18826a12d76624b3f8cdb0e280c1cfc74a0a341dda00f810ee911b87c5d" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="kk2QScKTs5ubWgHLshSXIaqxqt4OHyPoNOKs7BZXYgP34AMcXVYeDb1DTRAMA/FAiHqHKpt7EMKjaXMtIJd36Q==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-9bcf5def7eb44e2a101b20aaecf3707f4b0a10ab8f4d6eebec29371f821c4b29.css" media="all" rel="stylesheet" type="text/css" />
    <link href="https://assets-cdn.github.com/assets/github2-47bc67324d463c7cecb5ee4c009628c91db85b0e9288a9e663f2d06ff9e03088.css" media="all" rel="stylesheet" type="text/css" />
    
    


    <meta http-equiv="x-pjax-version" content="cffc32e08a29062b908cc3ddb47285af">

      
  <meta name="description" content="coursera-getting-cleaning-data - Repository for Getting and Cleaning Data Course Project ">
  <meta name="go-import" content="github.com/vasily_safroshkin/get_clean_data git https://github.com/vasily_safroshkin/get_clean_data.git">

  <meta content="38604" name="octolytics-dimension-user_id" /><meta content="vasily-safroshkin" name="octolytics-dimension-user_login" /><meta content="19879891" name="octolytics-dimension-repository_id" /><meta content="vasily_safroshkin/get_clean_data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="19879891" name="octolytics-dimension-repository_network_root_id" /><meta content="vasily_safroshkin/get_clean_data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/vasily_safroshkin/get_clean_data/commits/master.atom" rel="alternate" title="Recent Commits to coursera-getting-cleaning-data:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      
      


      <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" ga-data-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/vasily_safroshkin/get_clean_data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/vasily_safroshkin/get_clean_data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
      </div>
      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item explore">
          <a class="header-nav-link" href="/explore" data-ga-click="Header, go to explore, text:explore">Explore</a>
        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="Header, go to blog, text:blog">Blog</a>
          </li>
        <li class="header-nav-item">
          <a class="header-nav-link" href="https://help.github.com" data-ga-click="Header, go to help, text:help">Help</a>
        </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name" href="/vasily-safroshkin" data-ga-click="Header, go to profile, text:username">
      <img alt="vasily-safroshkin" class="avatar" data-user="9738662" height="20" src="https://avatars3.githubusercontent.com/u/9738662?v=3&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">vasily-safroshkin</span>
      </span>
    </a>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link js-menu-target tooltipped tooltipped-s" href="#" aria-label="Create new..." data-ga-click="Header, create new, icon:add">
      <span class="octicon octicon-plus"></span>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      
<ul class="dropdown-menu">
  <li>
    <a href="/new"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="vasily_safroshkin/get_clean_data">This repository</span>
    </li>
      <li>
        <a href="/vasily_safroshkin/get_clean_data/issues/new"><span class="octicon octicon-issue-opened"></span> New issue</a>
      </li>
</ul>

    </div>
  </li>

  <li class="header-nav-item">
        <a href="/notifications" aria-label="You have no unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:read" data-hotkey="g n">
        <span class="mail-status all-read"></span>
        <span class="octicon octicon-inbox"></span>
</a>
  </li>

  <li class="header-nav-item">
    <a class="header-nav-link tooltipped tooltipped-s" href="/settings/profile" id="account_settings" aria-label="Settings" data-ga-click="Header, go to settings, icon:settings">
      <span class="octicon octicon-gear"></span>
    </a>
  </li>

  <li class="header-nav-item">
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="LgZlIkINwojH9OH9NuTbB1x603HX2B/Ruqd/q+h5OGTdrCnYMgqrr/apexHHW+dAFQtjlN4RMI+83PkHbkaymA==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

      

        
<div class="flash-global js-notice flash-warn">
<div class="container">
    <h2>
      You don't have any verified emails.  We recommend <a href="https://github.com/settings/emails">verifying</a> at least one email.
    </h2>
    <p>
Email verification helps our support team verify ownership if you lose account access and allows you to receive all the notifications you ask for.
    </p>


















</div>
</div>


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

    <li class="subscription">
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="HpxovQinASIPR3Sx/IpdGo9iwq+fl2ZcXI+ZDPUVB6w4F4w400HhJ7XKMteEhYoNkdFDWStwmKz6mbOgjWDsuw==" /></div>  <input id="repository_id" name="repository_id" type="hidden" value="19879891" />

    <div class="select-menu js-menu-container js-select-menu">
      <a class="social-count js-social-count" href="/vasily_safroshkin/get_clean_data/watchers">
        1
      </a>
      <a href="/vasily_safroshkin/get_clean_data/subscription"
        class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true">
        <span class="js-select-button">
          <span class="octicon octicon-eye"></span>
          Watch
        </span>
      </a>

      <div class="select-menu-modal-holder">
        <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
          <div class="select-menu-header">
            <span class="select-menu-title">Notifications</span>
            <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
          </div> <!-- /.select-menu-header -->

          <div class="select-menu-list js-navigation-container" role="menu">

            <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                <h4>Not watching</h4>
                <span class="description">Be notified when participating or @mentioned.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Watch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                <h4>Watching</h4>
                <span class="description">Be notified of all conversations.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-eye"></span>
                  Unwatch
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

            <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <div class="select-menu-item-text">
                <input id="do_ignore" name="do" type="radio" value="ignore" />
                <h4>Ignoring</h4>
                <span class="description">Never be notified.</span>
                <span class="js-select-button-text hidden-select-button-text">
                  <span class="octicon octicon-mute"></span>
                  Stop ignoring
                </span>
              </div>
            </div> <!-- /.select-menu-item -->

          </div> <!-- /.select-menu-list -->

        </div> <!-- /.select-menu-modal -->
      </div> <!-- /.select-menu-modal-holder -->
    </div> <!-- /.select-menu -->

</form>
    </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/vasily_safroshkin/get_clean_data/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="UeoBgscZU3eHdpuXHDJ4mqLqtxB2fhBs/b/vEM4JcMSGewRazOZS07jGZuBjhv+XVbJRufGMVRy1ZZfKMTH4+g==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Unstar this repository" title="Unstar vasily_safroshkin/get_clean_data">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/vasily_safroshkin/get_clean_data/stargazers">
          0
        </a>
</form>
    <form accept-charset="UTF-8" action="/vasily_safroshkin/get_clean_data/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="89Md3/3c8xPD0Kfrv/Q0jClqhytDBkw1xgrprYZotrAhIlc7p5fBzTmP2uixXgHEhc1pUWxJdpesdnFhm66Xgw==" /></div>
      <button
        class="minibutton with-count js-toggler-target star-button"
        aria-label="Star this repository" title="Star vasily_safroshkin/get_clean_data">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/vasily_safroshkin/get_clean_data/stargazers">
          0
        </a>
</form>  </div>

  </li>


        <li>
          <a href="/vasily_safroshkin/get_clean_data/fork" class="minibutton with-count js-toggler-target fork-button tooltipped-n" title="Fork your own copy of vasily_safroshkin/get_clean_data to your account" aria-label="Fork your own copy of vasily_safroshkin/get_clean_data to your account" rel="nofollow" data-method="post">
            <span class="octicon octicon-repo-forked"></span>
            Fork
          </a>
          <a href="/vasily_safroshkin/get_clean_data/network" class="social-count">3</a>
        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/vasily-safroshkin" class="url fn" itemprop="url" rel="author"><span itemprop="title">vasily-safroshkin</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/vasily_safroshkin/get_clean_data" class="js-current-repository" data-pjax="#js-repo-pjax-container">coursera-getting-cleaning-data</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/vasily_safroshkin/get_clean_data/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/vasily_safroshkin/get_clean_data" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /vasily_safroshkin/get_clean_data">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/vasily_safroshkin/get_clean_data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /vasily_safroshkin/get_clean_data/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull Requests">
      <a href="/vasily_safroshkin/get_clean_data/pulls" aria-label="Pull Requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /vasily_safroshkin/get_clean_data/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull Requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>


      <li class="tooltipped tooltipped-w" aria-label="Wiki">
        <a href="/vasily_safroshkin/get_clean_data/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g w" data-selected-links="repo_wiki /vasily_safroshkin/get_clean_data/wiki">
          <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>
  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/vasily_safroshkin/get_clean_data/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /vasily_safroshkin/get_clean_data/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/vasily_safroshkin/get_clean_data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /vasily_safroshkin/get_clean_data/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>
  </ul>


</nav>

              <div class="only-with-full-nav">
                
  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/vasily_safroshkin/get_clean_data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="ssh"
  data-url="/users/set_protocol?protocol_selector=ssh&amp;protocol_type=clone">
  <h3><span class="text-emphasized">SSH</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="git@github.com:vasily_safroshkin/get_clean_data.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/vasily_safroshkin/get_clean_data" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<p class="clone-options">You can clone with
  <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a>, <a href="#" class="js-clone-selector" data-protocol="ssh">SSH</a>, or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>


  <a href="http://windows.github.com" class="minibutton sidebar-button" title="Save vasily_safroshkin/get_clean_data to your computer and use it in GitHub Desktop." aria-label="Save vasily_safroshkin/get_clean_data to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>

                <a href="/vasily_safroshkin/get_clean_data/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of vasily_safroshkin/get_clean_data as a zip file"
                   title="Download the contents of vasily_safroshkin/get_clean_data as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/vasily_safroshkin/get_clean_data/blob/27d81d0927f39cd57af8396b1a24c0810bae2434/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:eea483100e266848dfc522e0cd43d81d -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="minibutton select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div> <!-- /.select-menu-header -->

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div><!-- /.select-menu-tabs -->
      </div><!-- /.select-menu-filters -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item selected">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/vasily_safroshkin/get_clean_data/blob/master/CodeBook.md"
                 data-name="master"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="master">master</a>
            </div> <!-- /.select-menu-item -->
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div> <!-- /.select-menu-list -->

    </div> <!-- /.select-menu-modal -->
  </div> <!-- /.select-menu-modal-holder -->
</div> <!-- /.select-menu -->

  <div class="button-group right">
    <a href="/vasily_safroshkin/get_clean_data/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
  </div>

  <div class="breadcrumb js-zeroclipboard-target">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/vasily_safroshkin/get_clean_data" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">coursera-getting-cleaning-data</span></a></span></span><span class="separator">/</span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="Matti Lassila" class="avatar" data-user="38604" height="24" src="https://avatars0.githubusercontent.com/u/38604?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/vasily-safroshkin" rel="author">vasily-safroshkin</a></span>
        <time datetime="2014-05-25T16:32:13Z" is="relative-time">May 25, 2014</time>
        <div class="commit-title">
            <a href="/vasily_safroshkin/get_clean_data/commit/27d81d0927f39cd57af8396b1a24c0810bae2434" class="message" data-pjax="true" title="Typo correction">Typo correction</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="Matti Lassila" data-user="38604" height="24" src="https://avatars0.githubusercontent.com/u/38604?v=3&amp;s=48" width="24" />
            <a href="/vasily-safroshkin">vasily-safroshkin</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file-box">
  <div class="file">
    <div class="meta clearfix">
      <div class="info file-name">
          <span>63 lines (42 sloc)</span>
          <span class="meta-divider"></span>
        <span>2.37 kb</span>
      </div>
      <div class="actions">
        <div class="button-group">
          <a href="/vasily_safroshkin/get_clean_data/raw/master/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
            <a href="/vasily_safroshkin/get_clean_data/blame/master/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
          <a href="/vasily_safroshkin/get_clean_data/commits/master/CodeBook.md" class="minibutton " rel="nofollow">History</a>
        </div><!-- /.button-group -->

          <a class="octicon-button tooltipped tooltipped-nw"
             href="http://windows.github.com" aria-label="Open this file in GitHub for Windows">
              <span class="octicon octicon-device-desktop"></span>
          </a>

              <a class="octicon-button tooltipped tooltipped-n js-update-url-with-hash"
                 aria-label="Clicking this button will fork this project so you can edit the file"
                 href="/vasily_safroshkin/get_clean_data/edit/master/CodeBook.md"
                 data-method="post" rel="nofollow"><span class="octicon octicon-pencil"></span></a>

            <a class="octicon-button danger tooltipped tooltipped-s"
               href="/vasily_safroshkin/get_clean_data/delete/master/CodeBook.md"
               aria-label="Fork this project and delete file"
               data-method="post" data-test-id="delete-blob-file" rel="nofollow">
          <span class="octicon octicon-trashcan"></span>
        </a>
      </div><!-- /.actions -->
    </div>
    
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-getting-and-cleaning-data-coursera-course-project-codebook" class="anchor" href="#getting-and-cleaning-data-coursera-course-project-codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>Getting and Cleaning Data (Coursera). Course Project Codebook</h1>

<h2>
<a id="user-content-original-data" class="anchor" href="#original-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Original Data</h2>

<p>There original data comes from the smartphone accelerometer and gyroscope 3-axial raw signals, 
which have been processed using various signal processing techniques to measurement vector consisting
of 561 features. For detailed description of the original dataset, please see <code>features_info.txt</code> in
the zipped dataset file.</p>

<ul class="task-list">
<li>
<a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">source</a> </li>
<li><a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">description</a></li>
</ul>

<h2>
<a id="user-content-conventions-followed" class="anchor" href="#conventions-followed" aria-hidden="true"><span class="octicon octicon-link"></span></a>Conventions followed</h2>

<p>Processing code and dataset variable naming follows the conventions described in 
<a href="http://google-styleguide.googlecode.com/svn/trunk/Rguide.xml">Google R Styde Guide</a>.</p>

<h2>
<a id="user-content-data-sets" class="anchor" href="#data-sets" aria-hidden="true"><span class="octicon octicon-link"></span></a>Data sets</h2>

<h3>
<a id="user-content-raw-data-set" class="anchor" href="#raw-data-set" aria-hidden="true"><span class="octicon octicon-link"></span></a>Raw data set</h3>

<p>The raw dataset was created using the following regular expression to filter out required
features, eg. the measurements on the mean and standard deviation for each measurement
from the original feature vector set </p>

<p><code>-(mean|std)\\(</code></p>

<p>This regular expression selects 66 features from the original data set.
Combined with subject identifiers <code>subject</code> and activity labels <code>label</code>, this makes up the
68 variables of the processed raw data set.</p>

<p>The training and test subsets of the original dataset were combined to produce final raw dataset.</p>

<h3>
<a id="user-content-tidy-data-set" class="anchor" href="#tidy-data-set" aria-hidden="true"><span class="octicon octicon-link"></span></a>Tidy data set</h3>

<p>Tidy data set contains the average of all feature standard deviation and mean values of the raw dataset. 
Original variable names were modified in the follonwing way:</p>

<ol class="task-list">
<li>Replaced <code>-mean</code> with <code>Mean</code>
</li>
<li>Replaced <code>-std</code> with <code>Std</code>
</li>
<li>Removed parenthesis <code>-()</code>
</li>
<li>Replaced <code>BodyBody</code> with <code>Body</code>
</li>
</ol>

<p>It should be noted that the variable names are formatted in camelCase, as described in 
<a href="http://google-styleguide.googlecode.com/svn/trunk/Rguide.xml">Google R Styde Guide</a>. </p>

<h4>
<a id="user-content-sample-of-renamed-variables-compared-to-original-variable-name" class="anchor" href="#sample-of-renamed-variables-compared-to-original-variable-name" aria-hidden="true"><span class="octicon octicon-link"></span></a>Sample of renamed variables compared to original variable name</h4>

<table>
<thead>
<tr>
<th>Raw data</th>
<th>Tidy data</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>subject</code></td>
<td><code>subject</code></td>
</tr>
<tr>
<td><code>label</code></td>
<td><code>label</code></td>
</tr>
<tr>
<td><code>tBodyAcc-mean()-X</code></td>
<td><code>tBodyAccMeanX</code></td>
</tr>
<tr>
<td><code>tBodyAcc-mean()-Y</code></td>
<td><code>tBodyAccMeanY</code></td>
</tr>
<tr>
<td><code>tBodyAcc-mean()-Z</code></td>
<td><code>tBodyAccMeanZ</code></td>
</tr>
<tr>
<td><code>tBodyAcc-std()-X</code></td>
<td><code>tBodyAccStdX</code></td>
</tr>
<tr>
<td><code>tBodyAcc-std()-Y</code></td>
<td><code>tBodyAccStdY</code></td>
</tr>
<tr>
<td><code>tBodyAcc-std()-Z</code></td>
<td><code>tBodyAccStdZ</code></td>
</tr>
</tbody>
</table>
</article>
  </div>

  </div>
</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" class="js-jump-to-line-form">
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="button">Go</button>
  </form>
</div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
      <li><a href="https://status.github.com/">Status</a></li>
      <li><a href="https://developer.github.com">API</a></li>
      <li><a href="http://training.github.com">Training</a></li>
      <li><a href="http://shop.github.com">Shop</a></li>
      <li><a href="/blog">Blog</a></li>
      <li><a href="/about">About</a></li>

    </ul>

    <a href="/" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
    </a>

    <ul class="site-footer-links">
      <li>&copy; 2014 <span title="0.07846s from github-fe140-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="/site/terms">Terms</a></li>
        <li><a href="/site/privacy">Privacy</a></li>
        <li><a href="/security">Security</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
  </div><!-- /.site-footer -->
</div><!-- /.container -->


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents" placeholder=""></textarea>
      <div class="suggester-container">
        <div class="suggester fullscreen-suggester js-suggester js-navigation-container"></div>
      </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-fc447938e306b7b2c26a33cfee9dfda9052aeb1aa6ad84b72f1b35fd008efe9e.js" type="text/javascript"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-56c56f7fe2ed90ca50b9eefebccd56f3b9729a85d7ba17f0f9c9ebd02f20a7e3.js" type="text/javascript"></script>
      
      
  </body>
</html>

