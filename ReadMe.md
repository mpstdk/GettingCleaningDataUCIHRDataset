


<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>Coursera-Getting-and-Cleaning-Data/CodeBook.md at master · Xiaodan/Coursera-Getting-and-Cleaning-Data</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="twitter:title" /><meta content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data" name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" property="og:image" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" property="og:title" /><meta content="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data" property="og:url" /><meta content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data" property="og:description" />
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

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="CB37AD02:51F6:ECC0DAB:55095728" name="octolytics-dimension-request_id" /><meta content="11376660" name="octolytics-actor-id" /><meta content="mpstdk" name="octolytics-actor-login" /><meta content="3265256ac8be236437206ae9cfba35bb52b46fabab7e5d69e77ccd274bfd58e9" name="octolytics-actor-hash" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />

    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="Lyb3XU/7fASUZYF5WxF/k7JH0GGGiKfjLbSsI0O3G8PoEcmc9nHOua9W3pH1N3a0USkuDF+RQ8iUw09VslTf1w==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-53987f4912b4ff467e90fc72abf5fe32f6de81591135247ebe52a6e44240c22f.css" media="all" rel="stylesheet" />
    <link href="https://assets-cdn.github.com/assets/github2-5bff5ae06284ff2eb510dac0d4dba25b66ee6b9d5fdab323d6ab35bf6a0bd6a4.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="1d3fd441f9fad93ef7bcfd21888efc17">

      
  <meta name="description" content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data">
  <meta name="go-import" content="github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data git https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data.git">

  <meta content="1871047" name="octolytics-dimension-user_id" /><meta content="Xiaodan" name="octolytics-dimension-user_login" /><meta content="18748391" name="octolytics-dimension-repository_id" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="18748391" name="octolytics-dimension-repository_network_root_id" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data/commits/master.atom" rel="alternate" title="Recent Commits to Coursera-Getting-and-Cleaning-Data:master" type="application/atom+xml">

  </head>


  <body class="logged_in  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      


        <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <span class="mega-octicon octicon-mark-github"></span>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/Xiaodan/Coursera-Getting-and-Cleaning-Data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
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
    <a class="header-nav-link name" href="/mpstdk" data-ga-click="Header, go to profile, text:username">
      <img alt="@mpstdk" class="avatar" data-user="11376660" height="20" src="https://avatars3.githubusercontent.com/u/11376660?v=3&amp;s=40" width="20" />
      <span class="css-truncate">
        <span class="css-truncate-target">mpstdk</span>
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
    <a href="/new" data-ga-click="Header, create new repository, icon:repo"><span class="octicon octicon-repo"></span> New repository</a>
  </li>
  <li>
    <a href="/organizations/new" data-ga-click="Header, create new organization, icon:organization"><span class="octicon octicon-organization"></span> New organization</a>
  </li>


    <li class="dropdown-divider"></li>
    <li class="dropdown-header">
      <span title="Xiaodan/Coursera-Getting-and-Cleaning-Data">This repository</span>
    </li>
      <li>
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/issues/new" data-ga-click="Header, create new issue, icon:issue"><span class="octicon octicon-issue-opened"></span> New issue</a>
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
    <form accept-charset="UTF-8" action="/logout" class="logout-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="WIuLucV2WPm9k21BsqePf1hozrZFCEpU85MAQCTx2mkXdV0D9vMMA5HTIcaYgd4VaxweLTDBSzeUmGi03Tkczw==" /></div>
      <button class="header-nav-link sign-out-button tooltipped tooltipped-s" aria-label="Sign out" data-ga-click="Header, sign out, icon:logout">
        <span class="octicon octicon-sign-out"></span>
      </button>
</form>  </li>

</ul>


    
  </div>
</div>

        

        


      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

  <li>
      <form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="mA4xCZfSudlLX7Of6uL6kuBkbk/wevTuURJOux6jGhXWC74E2vWXVLZAt/6zIFjkKV6g34HQpPTwCdSYH1iZvg==" /></div>    <input id="repository_id" name="repository_id" type="hidden" value="18748391" />

      <div class="select-menu js-menu-container js-select-menu">
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/subscription"
          class="minibutton select-menu-button with-count js-menu-target" role="button" tabindex="0" aria-haspopup="true"
          data-ga-click="Repository, click Watch settings, action:blob#show">
          <span class="js-select-button">
            <span class="octicon octicon-eye"></span>
            Watch
          </span>
        </a>
        <a class="social-count js-social-count" href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/watchers">
          5
        </a>
        
        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header">
              <span class="select-menu-title">Notifications</span>
              <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
            </div>

            <div class="select-menu-list js-navigation-container" role="menu">

              <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input checked="checked" id="do_included" name="do" type="radio" value="included" />
                  <span class="select-menu-item-heading">Not watching</span>
                  <span class="description">Be notified when participating or @mentioned.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Watch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_subscribed" name="do" type="radio" value="subscribed" />
                  <span class="select-menu-item-heading">Watching</span>
                  <span class="description">Be notified of all conversations.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-eye"></span>
                    Unwatch
                  </span>
                </div>
              </div>

              <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                <span class="select-menu-item-icon octicon octicon-check"></span>
                <div class="select-menu-item-text">
                  <input id="do_ignore" name="do" type="radio" value="ignore" />
                  <span class="select-menu-item-heading">Ignoring</span>
                  <span class="description">Never be notified.</span>
                  <span class="js-select-button-text hidden-select-button-text">
                    <span class="octicon octicon-mute"></span>
                    Stop ignoring
                  </span>
                </div>
              </div>

            </div>

          </div>
        </div>
      </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/unstar" class="js-toggler-form starred js-unstar-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="vBd3B8swKuZ00Z8uPz+jQwbUKJV5zu6tviiTunOSx9Cq6qL+F9ezU04fZvTvidzBYbok/oIu/nezl5+l7MYzEQ==" /></div>
      <button
        class="minibutton with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar Xiaodan/Coursera-Getting-and-Cleaning-Data"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <span class="octicon octicon-star"></span>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/stargazers">
          10
        </a>
</form>
    <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/star" class="js-toggler-form unstarred js-star-button" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="2XIm0dqkNNI2S8NxF7P4P8IQ2Ko91Yd061Pa9ZnOATO7CEvcRfdYIhlcu82GhJS1mNchVvaTgV6/fEIDBGDf3g==" /></div>
      <button
        class="minibutton with-count js-toggler-target"
        aria-label="Star this repository" title="Star Xiaodan/Coursera-Getting-and-Cleaning-Data"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <span class="octicon octicon-star"></span>
        Star
      </button>
        <a class="social-count js-social-count" href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/stargazers">
          10
        </a>
</form>  </div>

  </li>

        <li>
          <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/fork" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="bgKs7w7iTT4vS6u4DGN/h9CFZEjCe24pbNaXLs6hyMNFleHQkK5Am994EDoHHCKSxfUz6ekKAftOFnGTu0bcMw==" /></div>
            <button
                type="submit"
                class="minibutton with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of Xiaodan/Coursera-Getting-and-Cleaning-Data to your account"
                aria-label="Fork your own copy of Xiaodan/Coursera-Getting-and-Cleaning-Data to your account">
              <span class="octicon octicon-repo-forked"></span>
              Fork
            </button>
            <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/network" class="social-count">127</a>
</form>        </li>

</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/Xiaodan" class="url fn" itemprop="url" rel="author"><span itemprop="title">Xiaodan</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" class="js-current-repository" data-pjax="#js-repo-pjax-container">Coursera-Getting-and-Cleaning-Data</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
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
     data-issue-count-url="/Xiaodan/Coursera-Getting-and-Cleaning-Data/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /Xiaodan/Coursera-Getting-and-Cleaning-Data">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /Xiaodan/Coursera-Getting-and-Cleaning-Data/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /Xiaodan/Coursera-Getting-and-Cleaning-Data/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>


      <li class="tooltipped tooltipped-w" aria-label="Wiki">
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/wiki" aria-label="Wiki" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g w" data-selected-links="repo_wiki /Xiaodan/Coursera-Getting-and-Cleaning-Data/wiki">
          <span class="octicon octicon-book"></span> <span class="full-word">Wiki</span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>      </li>
  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /Xiaodan/Coursera-Getting-and-Cleaning-Data/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /Xiaodan/Coursera-Getting-and-Cleaning-Data/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
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
           value="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data.git" readonly="readonly">
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
           value="git@github.com:Xiaodan/Coursera-Getting-and-Cleaning-Data.git" readonly="readonly">
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
           value="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data" readonly="readonly">
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


  <a href="github-windows://openRepo/https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data" class="minibutton sidebar-button" title="Save Xiaodan/Coursera-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop." aria-label="Save Xiaodan/Coursera-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>

                <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/archive/master.zip"
                   class="minibutton sidebar-button"
                   aria-label="Download the contents of Xiaodan/Coursera-Getting-and-Cleaning-Data as a zip file"
                   title="Download the contents of Xiaodan/Coursera-Getting-and-Cleaning-Data as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blob/68b24d6a77de3f755e6ab37ec6515df6687c8536/peer_assessment/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:1c838d70baa99e432b4b8b9de42784f7 -->

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
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blob/master/peer_assessment/CodeBook.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
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

  <div class="button-group right">
    <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/find/master"
          class="js-show-file-finder minibutton empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard minibutton zeroclipboard-button" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
  </div>

  <div class="breadcrumb js-zeroclipboard-target">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">Coursera-Getting-and-Cleaning-Data</span></a></span></span><span class="separator">/</span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/tree/master/peer_assessment" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">peer_assessment</span></a></span><span class="separator">/</span><strong class="final-path">CodeBook.md</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="Sally Zhang" class="avatar" data-user="1871047" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/Xiaodan" rel="author">Xiaodan</a></span>
        <time datetime="2014-04-27T02:34:48Z" is="relative-time">Apr 26, 2014</time>
        <div class="commit-title">
            <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/commit/b03135c5c504c16cd5fcd27c26dd3b411bcd6660" class="message" data-pjax="true" title="added codebook.r">added codebook.r</a>
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
            <img alt="Sally Zhang" data-user="1871047" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
            <a href="/Xiaodan">Xiaodan</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
    <div class="file-actions">
      <div class="button-group">
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/raw/master/peer_assessment/CodeBook.md" class="minibutton " id="raw-url">Raw</a>
          <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blame/master/peer_assessment/CodeBook.md" class="minibutton js-update-url-with-hash">Blame</a>
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/commits/master/peer_assessment/CodeBook.md" class="minibutton " rel="nofollow">History</a>
      </div><!-- /.button-group -->

        <a class="octicon-button tooltipped tooltipped-nw"
           href="github-windows://openRepo/https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data?branch=master&amp;filepath=peer_assessment%2FCodeBook.md" aria-label="Open this file in GitHub for Windows">
            <span class="octicon octicon-device-desktop"></span>
        </a>

            <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/edit/master/peer_assessment/CodeBook.md" aria-label="Clicking this button will fork this project so you can edit the file" class="tooltipped tooltipped-s inline-form edit-file-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="38WdhdkB/G8adrjUDUGBaktPeHWR7QxAB/HZeGzcS4MW1r5ckd8psFefM2fyyDcWI9jndj1//CorToi0OOPsxw==" /></div>
              <button class="web-edit-button"
                      type="submit"
                      data-hotkey="e"
                      data-disable-with>
                <span class="octicon octicon-pencil"></span>
              </button>
</form>
          <form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/delete/master/peer_assessment/CodeBook.md" aria-label="Fork this project and delete file" class="tooltipped tooltipped-s inline-form delete-file-form" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="O5QFIF+pPQqOC4iGmkr5Kjsf8J8DTLB4m3u8w8eizG3RpJJWNDvteboJPyOXISYHCPdZM3H9aRQnJ91hEXUpEQ==" /></div>
            <button class="web-edit-button"
                    type="submit"
                    data-disable-with>
              <span class="octicon octicon-trashcan "></span>
            </button>
</form>      </a>
    </div><!-- /.actions -->
    <div class="file-info">
        22 lines (21 sloc)
        <span class="file-info-divider"></span>
      3.147 kb
    </div>
  </div>
    <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-getting-and-cleaning-data-course-project-codebook" class="anchor" href="#getting-and-cleaning-data-course-project-codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>Getting and Cleaning Data Course Project CodeBook</h1>

<p>This file describes the variables, the data, and any transformations or work that I have performed to clean up the data.  </p>

<ul class="task-list">
<li>The site where the data was obtained:<br>
<a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a><br>
The data for the project:<br>
<a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a><br>
</li>
<li>The run_analysis.R script performs the following steps to clean the data:<br>

<ol class="task-list">
<li>Read X_train.txt, y_train.txt and subject_train.txt from the "./data/train" folder and store them in <em>trainData</em>, <em>trainLabel</em> and <em>trainSubject</em> variables respectively.<br>
</li>
<li>Read X_test.txt, y_test.txt and subject_test.txt from the "./data/test" folder and store them in <em>testData</em>, <em>testLabel</em> and <em>testsubject</em> variables respectively.<br>
</li>
<li>Concatenate <em>testData</em> to <em>trainData</em> to generate a 10299x561 data frame, <em>joinData</em>; concatenate <em>testLabel</em> to <em>trainLabel</em> to generate a 10299x1 data frame, <em>joinLabel</em>; concatenate <em>testSubject</em> to <em>trainSubject</em> to generate a 10299x1 data frame, <em>joinSubject</em>.<br>
</li>
<li>Read the features.txt file from the "/data" folder and store the data in a variable called <em>features</em>. We only extract the measurements on the mean and standard deviation. This results in a 66 indices list. We get a subset of <em>joinData</em> with the 66 corresponding columns.<br>
</li>
<li>Clean the column names of the subset. We remove the "()" and "-" symbols in the names, as well as make the first letter of "mean" and "std" a capital letter "M" and "S" respectively.<br>
</li>
<li>Read the activity_labels.txt file from the "./data"" folder and store the data in a variable called <em>activity</em>.<br>
</li>
<li>Clean the activity names in the second column of <em>activity</em>. We first make all names to lower cases. If the name has an underscore between letters, we remove the underscore and capitalize the letter immediately after the underscore.<br>
</li>
<li>Transform the values of <em>joinLabel</em> according to the <em>activity</em> data frame.<br>
</li>
<li>Combine the <em>joinSubject</em>, <em>joinLabel</em> and <em>joinData</em> by column to get a new cleaned 10299x68 data frame, <em>cleanedData</em>. Properly name the first two columns, "subject" and "activity". The "subject" column contains integers that range from 1 to 30 inclusive; the "activity" column contains 6 kinds of activity names; the last 66 columns contain measurements that range from -1 to 1 exclusive.<br>
</li>
<li>Write the <em>cleanedData</em> out to "merged_data.txt" file in current working directory.<br>
</li>
<li>Finally, generate a second independent tidy data set with the average of each measurement for each activity and each subject. We have 30 unique subjects and 6 unique activities, which result in a 180 combinations of the two. Then, for each combination, we calculate the mean of each measurement with the corresponding combination. So, after initializing the <em>result</em> data frame and performing the two for-loops, we get a 180x68 data frame.</li>
<li>Write the <em>result</em> out to "data_with_means.txt" file in current working directory. </li>
</ol>
</li>
</ul>

<p>© Xiaodan Zhang 2014 All Rights reserved.</p>
</article>
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
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.05146s from github-fe139-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
    </ul>
  </div>
</div>


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


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-d2f4f76d6a05f07ed67ef9f94d3823b34f98232770518bc7f8f40de8846ec511.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-f315a24d5d2e42f8e31bc3a92348625b7ccd168f4f3a33bb4977bf1a640448fa.js"></script>
      
      

  </body>
</html>

