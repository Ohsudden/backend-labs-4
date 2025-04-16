Password credential flow:

curl -X 'POST' \
'http://localhost:8080/realms/Volodymyr/protocol/openid-connect/token?' \
-H 'accept: application/json' \
-H 'Content-Type: application/x-www-form-urlencoded' \
-d 'grant_type=password&username=volodymyr&password=test&client_id=volodymyr-keycloak-client&client_secret=qJKomB7Hu40w7o43K1DxGLkBReXbN0Cf'

http://localhost:8080/realms/Volodymyr/protocol/openid-connect/token?


Response body

{
"access_token": "eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICI2ZlNWSWl4cFk1T2gwaGF6X3h2Tnl6QThwc3h3MUJ6R3FXSExmVEloZlNnIn0.eyJleHAiOjE3NDQ3OTUzMzQsImlhdCI6MTc0NDc5NTAzNCwianRpIjoib25ydHJvOjA1YzM3Nzc4LTFiZTgtNDc3YS1iNzQ3LTc0ZjExYmI4NjMzOSIsImlzcyI6Imh0dHA6Ly9sb2NhbGhvc3Q6ODA4MC9yZWFsbXMvVm9sb2R5bXlyIiwiYXVkIjoiYWNjb3VudCIsInN1YiI6IjRmYzg1NTMyLWM1ODAtNGRjOC1hMzUzLTU5M2FhM2FmYTFhYyIsInR5cCI6IkJlYXJlciIsImF6cCI6InZvbG9keW15ci1rZXljbG9hay1jbGllbnQiLCJzaWQiOiI0YzZiZDUyOS05ZWY5LTRkNTQtOTczMS00YzIwMjM4ZjQ0MTYiLCJhY3IiOiIxIiwiYWxsb3dlZC1vcmlnaW5zIjpbImh0dHA6bG9jYWxob3N0OjMwMDAiXSwicmVhbG1fYWNjZXNzIjp7InJvbGVzIjpbIm9mZmxpbmVfYWNjZXNzIiwiZGVmYXVsdC1yb2xlcy12b2xvZHlteXIiLCJ1bWFfYXV0aG9yaXphdGlvbiJdfSwicmVzb3VyY2VfYWNjZXNzIjp7ImFjY291bnQiOnsicm9sZXMiOlsibWFuYWdlLWFjY291bnQiLCJtYW5hZ2UtYWNjb3VudC1saW5rcyIsInZpZXctcHJvZmlsZSJdfX0sInNjb3BlIjoiZW1haWwgcHJvZmlsZSIsImVtYWlsX3ZlcmlmaWVkIjp0cnVlLCJuYW1lIjoiVm9sb2R5bXlyIFZ5c2huZXZldHNreWkiLCJwcmVmZXJyZWRfdXNlcm5hbWUiOiJ2b2xvZHlteXIiLCJnaXZlbl9uYW1lIjoiVm9sb2R5bXlyIiwiZmFtaWx5X25hbWUiOiJWeXNobmV2ZXRza3lpIiwiZW1haWwiOiJ2eXNobmV2ZXRza3lpdm9sb2R5bXlyQGdtYWlsLmNvbSJ9.jFaaH8UdVt1dGe9pxTX6sNOERXybF39FO4WwlrTgEeVnuG7aGh4cGuvZhC8DGit_A0xGGFb4o1faPhyTODWoAIwGR8aIkzuPZaifGcClwy7ROY-t132td0ewLqGrPFeK2ZqOWR8ybnlv4zSh2IXLMgCEQgpMHwpHrPYGVdkVAY38OXfhDjWwkWC4OzcBTaLAwdAPGLYVrOke8r3NXEfDxgJ1NyH_jg__R4Y5028GB7z6glqY57whSgFn93DZXtQR1Jv4HhUdKbABbNUXi7TQZeOcVSkvMJv98HBMiDldf50BHF1LU9AGWbHfdgXfggE6P4SbIKavDBE8FjzBFX4aIw",
"expires_in": 300,
"refresh_expires_in": 1800,
"refresh_token": "eyJhbGciOiJIUzUxMiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICI0NTI4ZDEwNi04NGYxLTQ5YTUtODBhOC0xNmU3M2RlMzQxMDUifQ.eyJleHAiOjE3NDQ3OTY4MzQsImlhdCI6MTc0NDc5NTAzNCwianRpIjoiZGVhZjgwNDgtM2MzNC00NjgyLTlkY2EtNWE4NDJiMzkzNDFmIiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9Wb2xvZHlteXIiLCJhdWQiOiJodHRwOi8vbG9jYWxob3N0OjgwODAvcmVhbG1zL1ZvbG9keW15ciIsInN1YiI6IjRmYzg1NTMyLWM1ODAtNGRjOC1hMzUzLTU5M2FhM2FmYTFhYyIsInR5cCI6IlJlZnJlc2giLCJhenAiOiJ2b2xvZHlteXIta2V5Y2xvYWstY2xpZW50Iiwic2lkIjoiNGM2YmQ1MjktOWVmOS00ZDU0LTk3MzEtNGMyMDIzOGY0NDE2Iiwic2NvcGUiOiJlbWFpbCB3ZWItb3JpZ2lucyBhY3Igc2VydmljZV9hY2NvdW50IHJvbGVzIHByb2ZpbGUgYmFzaWMifQ.rbIAFjs508BjMaWH2D1c-CgR1j283pqbX1775RinOqKiCJDtS-266xvjB4RXTsDav3l-7nS7i_GR3oJQlZx25w",
"token_type": "Bearer",
"not-before-policy": 0,
"session_state": "4c6bd529-9ef9-4d54-9731-4c20238f4416",
"scope": "email profile"
}

Client credential flow:

curl -X 'POST' \
'http://localhost:8080/realms/Volodymyr/protocol/openid-connect/token' \
-H 'accept: application/json' \
-H 'Content-Type: application/x-www-form-urlencoded' \
-d 'grant_type=client_credentials&client_id=volodymyr-keycloak-client&client_secret=qJKomB7Hu40w7o43K1DxGLkBReXbN0Cf'
Request URL
http://localhost:8080/realms/Volodymyr/protocol/openid-connect/token


Response body

{
"access_token": "eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICI2ZlNWSWl4cFk1T2gwaGF6X3h2Tnl6QThwc3h3MUJ6R3FXSExmVEloZlNnIn0.eyJleHAiOjE3NDQ3OTUyNTAsImlhdCI6MTc0NDc5NDk1MCwianRpIjoidHJydGNjOjU2ZmIxMWRhLTY2YmUtNDViMS1hY2FmLTBjMGZmNGI5MmVkOSIsImlzcyI6Imh0dHA6Ly9sb2NhbGhvc3Q6ODA4MC9yZWFsbXMvVm9sb2R5bXlyIiwiYXVkIjoiYWNjb3VudCIsInN1YiI6ImIwMTg5NDBlLTAxMWQtNGUyOC1iZTQ5LWUzODQ3YTAyMTJhNiIsInR5cCI6IkJlYXJlciIsImF6cCI6InZvbG9keW15ci1rZXljbG9hay1jbGllbnQiLCJhY3IiOiIxIiwiYWxsb3dlZC1vcmlnaW5zIjpbImh0dHA6bG9jYWxob3N0OjMwMDAiXSwicmVhbG1fYWNjZXNzIjp7InJvbGVzIjpbIm9mZmxpbmVfYWNjZXNzIiwiZGVmYXVsdC1yb2xlcy12b2xvZHlteXIiLCJ1bWFfYXV0aG9yaXphdGlvbiJdfSwicmVzb3VyY2VfYWNjZXNzIjp7ImFjY291bnQiOnsicm9sZXMiOlsibWFuYWdlLWFjY291bnQiLCJtYW5hZ2UtYWNjb3VudC1saW5rcyIsInZpZXctcHJvZmlsZSJdfX0sInNjb3BlIjoiZW1haWwgcHJvZmlsZSIsImNsaWVudEhvc3QiOiIxNzIuMTcuMC4xIiwiZW1haWxfdmVyaWZpZWQiOmZhbHNlLCJwcmVmZXJyZWRfdXNlcm5hbWUiOiJzZXJ2aWNlLWFjY291bnQtdm9sb2R5bXlyLWtleWNsb2FrLWNsaWVudCIsImNsaWVudEFkZHJlc3MiOiIxNzIuMTcuMC4xIiwiY2xpZW50X2lkIjoidm9sb2R5bXlyLWtleWNsb2FrLWNsaWVudCJ9.Bcyc0PKQGHa3gxHtwlMyEpR1CzVP-kiqXCl2NhYsp54gfM7vNRNJXIJlSDZiwNe6QIcyFPXrnCDFYGkeY-zwN5wEHtMtEOXQAJSBGiEi1u1SgqUWMPf5YAuW86gs27swaCJuwy2p6OAN5GX49Xcqyr-6rWrAtsP0-bP2Y0_GmSmAhcZIFUnTWLtbPZK2IaBkZs69WJ1zGp29efUAoaVNJ9QdcTFKbEmiZu-LWCyK3SWc0tYmWWSAEdlWwDyvc3gao1awDKrXFgFb0RgNWriqSO9nBz6soYzdoGl3WrXzVFv4oAe8uS0MMu9dsK0UqdubjwQjQvvO8cdDh0pAXv08Vw",
"expires_in": 300,
"refresh_expires_in": 0,
"token_type": "Bearer",
"not-before-policy": 0,
"scope": "email profile"
}

Authorization flow:

curl -X 'GET' \
'http://localhost:8080/realms/Volodymyr/protocol/openid-connect/auth?response_type=code&client_id=volodymyr-keycloak-client&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid' \
-H 'accept: */*'

http://localhost:8080/realms/Volodymyr/protocol/openid-connect/auth?response_type=code&client_id=volodymyr-keycloak-client&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid

Response body

<!DOCTYPE html>
<html class="login-pf" lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <meta name="robots" content="noindex, nofollow">
    <meta name="color-scheme" content="light dark">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <title>Sign in to Volodymyr</title>
    <link rel="icon" href="/resources/ztvdq/login/keycloak.v2/img/favicon.ico" />
            <link href="/resources/ztvdq/common/keycloak/vendor/patternfly-v5/patternfly.min.css" rel="stylesheet" />
            <link href="/resources/ztvdq/common/keycloak/vendor/patternfly-v5/patternfly-addons.css" rel="stylesheet" />
            <link href="/resources/ztvdq/login/keycloak.v2/css/styles.css" rel="stylesheet" />
    <script type="importmap">
        {
            "imports": {
                "rfc4648": "/resources/ztvdq/common/keycloak/vendor/rfc4648/rfc4648.js"
            }
        }
    </script>
      <script type="module" async blocking="render">
          const DARK_MODE_CLASS = "pf-v5-theme-dark";
          const mediaQuery = window.matchMedia("(prefers-color-scheme: dark)");

          updateDarkMode(mediaQuery.matches);
          mediaQuery.addEventListener("change", (event) => updateDarkMode(event.matches));

          function updateDarkMode(isEnabled) {
            const { classList } = document.documentElement;

            if (isEnabled) {
              classList.add(DARK_MODE_CLASS);
            } else {
              classList.remove(DARK_MODE_CLASS);
            }
          }
      </script>
    <script type="module" src="/resources/ztvdq/login/keycloak.v2/js/passwordVisibility.js"></script>
    <script type="module">
        import { startSessionPolling } from "/resources/ztvdq/login/keycloak.v2/js/authChecker.js";

        startSessionPolling(
            "/realms/Volodymyr/login-actions/restart?client_id=volodymyr-keycloak-client&tab_id=0c0dxN69JN4&client_data=eyJydSI6Imh0dHA6Ly9sb2NhbGhvc3Q6MzAwMC9jYWxsYmFjayIsInJ0IjoiY29kZSJ9&skip_logout=true"
        );
    </script>
        <script type="module">
            import { checkAuthSession } from "/resources/ztvdq/login/keycloak.v2/js/authChecker.js";

            checkAuthSession(
                "CXyx91iMv2jNPxFlM5jbMs9aik3W93bVy6aQmzyo544"
            );
        </script>
    <script>
      // Workaround for https://bugzilla.mozilla.org/show_bug.cgi?id=1404468
      const isFirefox = true;
    </script>
</head>

<body id="keycloak-bg" class="" data-page-id="login-login">
<div class="pf-v5-c-login">
  <div class="pf-v5-c-login__container">
    <header id="kc-header" class="pf-v5-c-login__header">
      <div id="kc-header-wrapper"
              class="pf-v5-c-brand">Volodymyr</div>
    </header>
    <main class="pf-v5-c-login__main">
      <div class="pf-v5-c-login__main-header">
        <h1 class="pf-v5-c-title pf-m-3xl" id="kc-page-title"><!-- template: login.ftl -->

        Sign in to your account

</h1>
      </div>
      <div class="pf-v5-c-login__main-body">


<!-- template: login.ftl -->

        <div id="kc-form">
          <div id="kc-form-wrapper">
                <form id="kc-form-login" class="pf-v5-c-form pf-v5-u-w-100" onsubmit="login.disabled = true; return true;" action="http://localhost:8080/realms/Volodymyr/login-actions/authenticate?session_code=ZCAqReKLP98jOfnKXn8bY990f5KJE2fr_IPUqjJbf1A&amp;execution=3b3ec7c0-703c-41a7-a4a9-299541ed4126&amp;client_id=volodymyr-keycloak-client&amp;tab_id=0c0dxN69JN4&amp;client_data=eyJydSI6Imh0dHA6Ly9sb2NhbGhvc3Q6MzAwMC9jYWxsYmFjayIsInJ0IjoiY29kZSJ9" method="post" novalidate="novalidate">

<div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__group-label pf-v5-u-pb-xs">
        <label for="username" class="pf-v5-c-form__label">
        <span class="pf-v5-c-form__label-text">
                                        Username or email

        </span>
        </label>
    </div>

    <span class="pf-v5-c-form-control ">
        <input id="username" name="username" value="" type="text" autocomplete="username" autofocus
                aria-invalid=""/>
    </span>

    <div id="input-error-container-username">
    </div>
</div>


<div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__group-label pf-v5-u-pb-xs">
        <label for="password" class="pf-v5-c-form__label">
        <span class="pf-v5-c-form__label-text">
            Password
        </span>
        </label>
    </div>

    <div class="pf-v5-c-input-group">
      <div class="pf-v5-c-input-group__item pf-m-fill">
        <span class="pf-v5-c-form-control ">
          <input id="password" name="password" value="" type="password" autocomplete="current-password" 
                  aria-invalid=""/>
        </span>
      </div>
      <div class="pf-v5-c-input-group__item">
        <button class="pf-v5-c-button pf-m-control" type="button" aria-label="Show password"
                aria-controls="password" data-password-toggle
                data-icon-show="fa-eye fas" data-icon-hide="fa-eye-slash fas"
                data-label-show="Show password" data-label-hide="Hide password">
            <i class="fa-eye fas" aria-hidden="true"></i>
        </button>
      </div>
    </div>
    <div class="pf-v5-c-form__helper-text" aria-live="polite">
        <div class="pf-v5-c-helper-text pf-v5-u-display-flex pf-v5-u-justify-content-space-between">
        </div>
    </div>


    <div id="input-error-container-password">
    </div>
</div>


                    <input type="hidden" id="id-hidden-input" name="credentialId" />
  <div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__actions pf-v5-u-pt-xs pf-v5-u-flex-wrap">
  <button class="pf-v5-c-button pf-m-primary pf-m-block " name="login" id="kc-login"
          type="submit" >
  Sign In
  </button>
    </div>
  </div>
                </form>
            </div>
        </div>



          <div class="pf-v5-c-login__main-footer">
<!-- template: login.ftl -->



          </div>
      </div>

        <div class="pf-v5-c-login__main-footer">
        </div>
    </main>
  </div>
</div>
</body>
</html>
Response headers
 access-control-allow-credentials: true 
 access-control-allow-origin: http://localhost:58182 
 cache-control: no-store,must-revalidate,max-age=0 
 content-language: en 
 content-length: 6128 
 content-security-policy: frame-src 'self'; frame-ancestors 'self'; object-src 'none'; 
 content-type: text/html;charset=utf-8 
 referrer-policy: no-referrer 
 strict-transport-security: max-age=31536000; includeSubDomains 
 vary: origin 
 x-content-type-options: nosniff 
 x-frame-options: SAMEORIGIN 
 x-robots-tag: none

Implicit Flow:

curl -X 'GET' \
'http://localhost:8080/realms/Volodymyr/protocol/openid-connect/auth?response_type=token&client_id=volodymyr-keycloak-client&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid' \
-H 'accept: */*'
Request URL
http://localhost:8080/realms/Volodymyr/protocol/openid-connect/auth?response_type=token&client_id=volodymyr-keycloak-client&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid

Response body

<!DOCTYPE html>
<html class="login-pf" lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <meta name="robots" content="noindex, nofollow">
    <meta name="color-scheme" content="light dark">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <title>Sign in to Volodymyr</title>
    <link rel="icon" href="/resources/ztvdq/login/keycloak.v2/img/favicon.ico" />
            <link href="/resources/ztvdq/common/keycloak/vendor/patternfly-v5/patternfly.min.css" rel="stylesheet" />
            <link href="/resources/ztvdq/common/keycloak/vendor/patternfly-v5/patternfly-addons.css" rel="stylesheet" />
            <link href="/resources/ztvdq/login/keycloak.v2/css/styles.css" rel="stylesheet" />
    <script type="importmap">
        {
            "imports": {
                "rfc4648": "/resources/ztvdq/common/keycloak/vendor/rfc4648/rfc4648.js"
            }
        }
    </script>
      <script type="module" async blocking="render">
          const DARK_MODE_CLASS = "pf-v5-theme-dark";
          const mediaQuery = window.matchMedia("(prefers-color-scheme: dark)");

          updateDarkMode(mediaQuery.matches);
          mediaQuery.addEventListener("change", (event) => updateDarkMode(event.matches));

          function updateDarkMode(isEnabled) {
            const { classList } = document.documentElement;

            if (isEnabled) {
              classList.add(DARK_MODE_CLASS);
            } else {
              classList.remove(DARK_MODE_CLASS);
            }
          }
      </script>
    <script type="module" src="/resources/ztvdq/login/keycloak.v2/js/passwordVisibility.js"></script>
    <script type="module">
        import { startSessionPolling } from "/resources/ztvdq/login/keycloak.v2/js/authChecker.js";

        startSessionPolling(
            "/realms/Volodymyr/login-actions/restart?client_id=volodymyr-keycloak-client&tab_id=XATDldKXKz0&client_data=eyJydSI6Imh0dHA6Ly9sb2NhbGhvc3Q6MzAwMC9jYWxsYmFjayIsInJ0IjoidG9rZW4ifQ&skip_logout=true"
        );
    </script>
        <script type="module">
            import { checkAuthSession } from "/resources/ztvdq/login/keycloak.v2/js/authChecker.js";

            checkAuthSession(
                "VMEHK/X3hUa2fgwuK6RlGVnlu/lxE0Yp+pg9O+4vUWs"
            );
        </script>
    <script>
      // Workaround for https://bugzilla.mozilla.org/show_bug.cgi?id=1404468
      const isFirefox = true;
    </script>
</head>

<body id="keycloak-bg" class="" data-page-id="login-login">
<div class="pf-v5-c-login">
  <div class="pf-v5-c-login__container">
    <header id="kc-header" class="pf-v5-c-login__header">
      <div id="kc-header-wrapper"
              class="pf-v5-c-brand">Volodymyr</div>
    </header>
    <main class="pf-v5-c-login__main">
      <div class="pf-v5-c-login__main-header">
        <h1 class="pf-v5-c-title pf-m-3xl" id="kc-page-title"><!-- template: login.ftl -->

        Sign in to your account

</h1>
      </div>
      <div class="pf-v5-c-login__main-body">


<!-- template: login.ftl -->

        <div id="kc-form">
          <div id="kc-form-wrapper">
                <form id="kc-form-login" class="pf-v5-c-form pf-v5-u-w-100" onsubmit="login.disabled = true; return true;" action="http://localhost:8080/realms/Volodymyr/login-actions/authenticate?session_code=-SLvO_VKQ3B23HBjsIj4qa9NjYHPpb5fM4uClz8wTo0&amp;execution=3b3ec7c0-703c-41a7-a4a9-299541ed4126&amp;client_id=volodymyr-keycloak-client&amp;tab_id=XATDldKXKz0&amp;client_data=eyJydSI6Imh0dHA6Ly9sb2NhbGhvc3Q6MzAwMC9jYWxsYmFjayIsInJ0IjoidG9rZW4ifQ" method="post" novalidate="novalidate">

<div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__group-label pf-v5-u-pb-xs">
        <label for="username" class="pf-v5-c-form__label">
        <span class="pf-v5-c-form__label-text">
                                        Username or email

        </span>
        </label>
    </div>

    <span class="pf-v5-c-form-control ">
        <input id="username" name="username" value="" type="text" autocomplete="username" autofocus
                aria-invalid=""/>
    </span>

    <div id="input-error-container-username">
    </div>
</div>


<div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__group-label pf-v5-u-pb-xs">
        <label for="password" class="pf-v5-c-form__label">
        <span class="pf-v5-c-form__label-text">
            Password
        </span>
        </label>
    </div>

    <div class="pf-v5-c-input-group">
      <div class="pf-v5-c-input-group__item pf-m-fill">
        <span class="pf-v5-c-form-control ">
          <input id="password" name="password" value="" type="password" autocomplete="current-password" 
                  aria-invalid=""/>
        </span>
      </div>
      <div class="pf-v5-c-input-group__item">
        <button class="pf-v5-c-button pf-m-control" type="button" aria-label="Show password"
                aria-controls="password" data-password-toggle
                data-icon-show="fa-eye fas" data-icon-hide="fa-eye-slash fas"
                data-label-show="Show password" data-label-hide="Hide password">
            <i class="fa-eye fas" aria-hidden="true"></i>
        </button>
      </div>
    </div>
    <div class="pf-v5-c-form__helper-text" aria-live="polite">
        <div class="pf-v5-c-helper-text pf-v5-u-display-flex pf-v5-u-justify-content-space-between">
        </div>
    </div>


    <div id="input-error-container-password">
    </div>
</div>


                    <input type="hidden" id="id-hidden-input" name="credentialId" />
  <div class="pf-v5-c-form__group">
    <div class="pf-v5-c-form__actions pf-v5-u-pt-xs pf-v5-u-flex-wrap">
  <button class="pf-v5-c-button pf-m-primary pf-m-block " name="login" id="kc-login"
          type="submit" >
  Sign In
  </button>
    </div>
  </div>
                </form>
            </div>
        </div>



          <div class="pf-v5-c-login__main-footer">
<!-- template: login.ftl -->



          </div>
      </div>

        <div class="pf-v5-c-login__main-footer">
        </div>
    </main>
  </div>
</div>
</body>
</html>