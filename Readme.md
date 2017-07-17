technical
=========
Would recommend this for small and medium size projects (less than 50)

```
/src
    /lib/           - utility, helper, monkey-patched libs, etc
    /services       - everything that belongs in the datalayer (graphql schema, api communication, authorization)
    /elements/      - pure dump components like Button, Label, Popup, Logo - things you would possibly put or use from an external lib (ui-lib)
    /components/    - re-usable components with optional data-binding
    /pages/         - everything that has a route = pages with router configuration (subroutes as subdirs - see react-router examples)
    /theme          - theme/base-styles
/bin                - build-scripts, config
/dist               - build artifacts, app, server, coverage results, etc
/test
    /e2e            - end2end tests - smoke-tests and full-testsuite
    /unit           - unit tests
```
    


modules
=======
Every module would maintain their own structure and tests - you can think basically about a module like a npm-package on its own

```
/lib/           - utility, helper, monkey-patched libs, xyz
/modules
    - app - base app module with layout, configuration 
    - base (pure dump components like Button, Label, Popup - things you would possibly put or use from an external lib (ui-lib))
    - teaser
    - search(filter)
    - theme
/bin                - build-scripts, config
/dist               - build artifacts, app, server, coverage results, etc
/test
    /e2e            - end2end tests - smoke-tests and full-testsuite
```
