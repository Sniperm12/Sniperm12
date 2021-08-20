/**
 * @name OperaGxGamingTheme
 * @author TomRdh
 * @version 0.0.9
 * @description Opera GX Gaming Theme! A (transparent) gaming theme inspired by Opera GX. Very customizable in the theme file.
 * @website https://tomrdh.github.io/da-website/main
 * @source https://github.com/Tomrdh/discord-addons/blob/master/download-themes-here/OperaGxGamingTheme
 * @invite v7ECsqT
 * @authorId 703638166162112516
*/

/* Import CSS link(s) */
@import url(https://tomrdh.github.io/discord-addons/xcores/themes/OGGT_Core.css);

:root { /* Theme-Settings */
/*  Variable Name                   | Variable Value                        | | Default Value(s)                                               | About This Variable (alias: Setting)                                                                                                                                                                           */

/*  Background-Settings                                                                                                                                                                                                                                                                                                                                         */
    --background:                     var(--opera-gx-bg-1)                  ;/* Default: var(--opera-gx-bg-1)                                  - Background for app-mount, you can use a preset var, your own url, transparent (requires transparency enabled and dark theme set) or just a color. Var syntax: var(--var-name), url syntax: url(https://…).     */
    --background-behind-appmount:     rgb(var(--darker-background-color))   ;/* Default: rgb(var(--darker-background-color))                   - Background that is behind the --background variable, in case if --background is unloaded. To make your app transparent, set BOTH background variables to transparent. Otehrwise, put a background color.       */
    
/*  Color-Settings (RGB only)                                                                                                                                                                                                                                                                                                                                   */
    --accent-color-1:                 250, 30, 70                           ;/* Default: 250, 30, 70                                           - The main accent color used in the theme.                                                                                                                                                                       */
    --accent-color-2:                 255, 55, 109                          ;/* Default: 255, 55, 109                                          - This 2nd one should be a bit lighter or darker than the first one. But anyways you can use the color you want, some gradients can be very awesome.                                                             */
    --dark-background-color:          18, 16, 25                            ;/* Default: 18, 16, 25                                            - Background color used in some elements, like the chatbox.                                                                                                                                                      */
    --darker-background-color:        8, 5, 14                              ;/* Default: 8, 5, 14                                              - Another background color, this is darker than --dark-background-color.                                                                                                                                         */

/*  More-Color-Settings                                                                                                                                                                                                                                                                                                                                         */
    --gx-red:                         255, 34, 34                           ;/* Theme Default: 255, 34, 34   - Discord Default: 240, 71, 71    - Main red color when using the theme. The second one should be brighter than the first one, just like the secondary accent color.                                                                               */
    --gx-red-2:                       255, 66, 66                           ;/* Default: 255, 66, 66                                           - Secondary red color when using the theme.                                                                                                                                                                      */
    --gx-yellow:                      234, 234, 34                          ;/* Theme Default: 234, 234, 34  - Discord Default: 250, 166, 26   - Main yellow color when using the theme.                                                                                                                                                                        */
    --gx-yellow-2:                    255, 255, 68                          ;/* Default: 255, 255, 68                                          - Secondary yellow color when using the theme.                                                                                                                                                                   */
    --gx-green:                       0, 212, 81                            ;/* Theme Default: 0, 212, 81    - Discord Default: 67, 181, 129   - Main green color when using the theme.                                                                                                                                                                         */
    --gx-green-2:                     0, 255, 129                           ;/* Default: 0, 255, 129                                           - Secondary green color when using the theme.                                                                                                                                                                    */

/*  Font-Color-Settings                                                                                                                                                                                                                                                                                                                                         */
    --fullwhite-font:                 250, 253, 255                         ;/* Default: 250, 253, 255                                         - Color used for texts with the full white color. Note that these vars also modify some icons.                                                                                                                   */
    --normal-font:                    201, 203, 206                         ;/* Theme Default: 201, 203, 206 - Discord Default: 185, 187, 190  - Color used for texts with the normal white color.                                                                                                                                                              */
    --normal-hover-font:              238, 239, 240                         ;/* Theme Default: 238, 239, 240 - Discord Default: 220, 221, 222  - Color used for texts with the white color when hovering.                                                                                                                                                       */
    --muted-font:                     114, 118, 125                         ;/* Default: 114, 118, 125                                         - Muted text is commonly darker than the normal text color.                                                                                                                                                      */
    --link-text:                      0, 176, 244                           ;/* Default: 0, 176, 244                                           - Color used for links.                                                                                                                                                                                          */
    --font-in-accent:                 0, 0, 0                               ;/* Default: 0, 0, 0                                               - Color used for text and icons that are in a element that has the --accent-color-X variable as a background color.                                                                                              */

/*  Font-Setting                                                                                                                                                                                                                                                                                                                                                */
    --channel-name-transform:         capitalize                            ;/* Theme Default: capitalize    - Discord Default: unset          - Decide if you want to use uppercase or lowercase characters in channel names. Values: unset, lowercase, uppercase, capitalize.                                                                                 */
    --category-name-transform:        unset                                 ;/* Theme Default: unset         - Discord Default: uppercase      - Same as channel names but for categories. Same values.                                                                                                                                                         */

/*  Advanced-Background-Settings                                                                                                                                                                                                                                                                                                                                */
    --wintitlebar-background-blur:    none                                  ;/* Default: none                                                  - Background blur for the Windows title bar. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                               */
    --wintitlebar-transparency:       0.7                                   ;/* Default: 0.7                                                   - Transparency for the Windows title bar. Between 0 and 1.                                                                                                                                                       */
    --wintitlebar-transparency-color: var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */
    --wintb-focused-alpha:            1                                     ;/* Default: 1                                                     - Transparency for the Windows title bar when the app is focused. Between 0 and 1.                                                                                                                               */
    --wintb-focused-color:            var(--darker-background-color)        ;/* Default: var(--darker-background-color)                        - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --header-background-blur:         none                                  ;/* Default: none                                                  - Background blur for header. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                              */
    --header-transparency:            0.3                                   ;/* Default: 0.3                                                   - Transparency for header. Between 0 and 1.                                                                                                                                                                      */
    --header-transparency-color:      var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --serverlist-background-blur:     none                                  ;/* Default: none                                                  - Background blur for server list. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                         */
    --serverlist-transparency:        0                                     ;/* Default: 0                                                     - Transparency for server list. Between 0 and 1.                                                                                                                                                                 */
    --serverlist-transparency-color:  var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --channels-background-blur:       none                                  ;/* Default: none                                                  - Background blur for channel list. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                        */
    --channels-transparency:          0                                     ;/* Default: 0                                                     - Transparency for channel list. Between 0 and 1.                                                                                                                                                                */
    --channels-transparency-color:    var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --chat-background-blur:           none                                  ;/* Default: none                                                  - Background blur for header. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                              */
    --chat-transparency:              0                                     ;/* Default: 0                                                     - Transparency for chat window. Between 0 and 1.                                                                                                                                                                 */
    --chat-transparency-color:        var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --memberlist-background-blur:     none                                  ;/* Default: none                                                  - Background blur for member list. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                         */
    --memberlist-transparency:        0                                     ;/* Default: 0                                                     - Transparency for member list. Between 0 and 1.                                                                                                                                                                 */
    --memberlist-transparency-color:  var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - RGB color used if transparency is higher than 0.                                                                                                                                                               */

    --st-l-scroller-bg-blur:          none                                  ;/* Default: none                                                  - Background blur for settings sidebar using any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                   */
    --st-l-scroller-transparency:     1                                     ;/* Default: 1                                                     - Background transparency for settings sidebar between 0 and 1.                                                                                                                                                  */
    --st-l-scroller-color:            var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - Background color for settings sidebar if transparency is higher than 0.                                                                                                                                        */
    --st-r-scroller-bg-blur:          none                                  ;/* Default: none                                                  - Background blur for settings content using any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                                   */
    --st-r-scroller-transparency:     1                                     ;/* Default: 1                                                     - Background transparency for settings content between 0 and 1.                                                                                                                                                  */
    --st-r-scroller-color:            var(--darker-background-color)        ;/* Default: var(--darker-background-color)                        - Background color for settings content if transparency is higher than 0.                                                                                                                                        */

/*  Advanced-Element-Transparency-Settings                                                                                                                                                                                                                                                                                                                      */
    --chatbox-transparency:           1                                     ;/* Default: 1                                                     - Background transparency for the chat box when not focused.                                                                                                                                                     */
    --chatbox-focused-transparency:   1                                     ;/* Default: 1                                                     - Background transparency for the chat box when focused.                                                                                                                                                         */
    --other-transparency:             1                                     ;/* Default: 1                                                     - Background transparency for other things.                                                                                                                                                                      */
    --other-highlighted-transparency: 1                                     ;/* Default: 1                                                     - Background transparency for other things when hovered/focused/active/etc.                                                                                                                                      */
    --lines-transparency:             1                                     ;/* Default: 1                                                     - Transparency for lines using the first accent color.                                                                                                                                                           */

/*  Plugin-Compatibility-Settings                                                                                                                                                                                                                                                                                                                               */
    --channeltabs-background-color:   var(--darker-background-color)        ;/* Default: var(--darker-background-color)                        - Background color for ChannelTabs TabContainer.                                                                                                                                                                 */
    --channeltabs-background-blur:    none                                  ;/* Default: none                                                  - Background blur for ChannelTabs TabContainer. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                            */
    --channeltabs-bg-transparency:    1                                     ;/* Default: 1                                                     - Variable for the ChannelTabs plugin style. Background transparency for the TabContainer.                                                                                                                       */
    --channeltabs-tab-bg-color:       var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - Background color for the selected tab.                                                                                                                                                                         */
    --channeltabs-tab-bg-transparency:1                                     ;/* Default: 1                                                     - Variable for the ChannelTabs plugin style. Background transparency for the selected tab.                                                                                                                       */

    --channeltabs-fav-bg-color:       var(--dark-background-color)          ;/* Default: var(--dark-background-color)                          - Background color for ChannelTabs FavContainer.                                                                                                                                                                 */
    --channeltabs-fav-bg-blur:        none                                  ;/* Default: none                                                  - Background blur for ChannelTabs TabContainer. Use any unit supported by CSS like px. Put none to remove blur effect and avoid lags.                                                                            */
    --channeltabs-fav-bg-transparency:1                                     ;/* Default: 1                                                     - Variable for the ChannelTabs plugin style. Background transparency for the FavContainer.                                                                                                                       */
    --channeltabs-fav-hover:          111, 125, 138                         ;/* Default: 111, 125, 138                                         - Background color when you hover on a favorite.                                                                                                                                                                 */
    --channeltabs-fav-hover-alpha:    0.3                                   ;/* Default: 0.3                                                   - Background transparency when you hover on a favorite.                                                                                                                                                          */

/*  /!\ Update-setting (DO NOT MODIFY OR REMOVE) /!\  */
    --version008_oggt: none; /* Do not modify nor remove this variable, or you'll see an annoying notice that tells you to redownload the theme!                                                                                                                                                                                                                */
}

/*  Custom-CSS                                                                                                                                                                                                                                                                                                                                                  */
/*  You can put Custom CSS just below. If you're trying to fix an issue, feel free to also report it to me, so it can be fixed for everyone.                                                                                                                                                                                                                    */
