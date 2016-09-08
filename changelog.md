# Changelog

### v0.7.0, 2016-07-01
 * added: compact mode, hide text labels on tabs for a minimal tab sidebar (#55)
 * added: preference to display tab toolbar at top (new default) or at bottom (#46)
 * themes improvements:
   * Dark, Light themes:
     * more subtle (smaller and less contrast) splitter between tab sidebar and website (#21)
   * template Basic, Dark theme:
     * fixed: don't show close button on pinned tabs
   * template Basic:
     * internal: accept all kind of background values
 * internal: don't spam the console anymore for good
 * internal: mark as compatible with e10s


***


### v0.6.2, 2016-05-31
 * added: compatibility to Tab Mix Plus v0.5 or newer (#19)


***


### v0.6.1, 2016-05-08
 * themes improvements:
   * the Dark (default) and Light themes are now official recommended
   * all themes:
     * remove all statuspanel related styles
   * Darwin, Linux, Windows themes:
     * add blue left border to pinned tabs (#32)
 * fixed: don't spam the console with debug output
 * internal: some refactoring for more efficient code 


***


### v0.6.0, 2016-05-06
 * added: button to toggle `browser.tabs.drawInTitlebar` for the case that window control elements are overlappig with FF (#9)
   * note: this is set automatically to `true` once at installation
 * added: possibility to reset VTR preferences to default via button (#11)
 * fixed: hotkey to hide tabbar only works in the latest opened window (#30)
 * fixed: destroy references to closed windows, set memory free (#39)
 * themes improvements:
   * all themes (except Darwin):
     * fixed: status bar was not readable on some Linux desktops (e.g. KDE) (#37)
   * no theme option:
     * the base style rules are including now a border between tabs and a min and max height of tabs
   * Dark theme:
     * fixed: Close button shown thrice under some circumstances (#35)
 * intern: rename object to VerticalTabsReloaded (before: VerticalTabs)


***


### v0.5.0, 2016-03-31
 * themes improvements:
   * all themes:
     * all themes have now a border between tabs (#24)
	 * show Firefox placeholder favicon if the tab has none instead of no icon at all (#25)
	 * internal: remove unnecessary style rules
   * internal: introduced templates
	 * create and adapt easily a theme without worrying too much about css
	 * if a templates get bug fixes or enhancements all themes building on it are profiting
	 * templates might be also the foundation for full user customization of themes in the future
	 * created a template named Basic, based on the Dark Theme style
   * introduce option to choose no theme
     * this might be a good option to let other add-ons decide tab colors, font attributes etc.
   * Darwin theme:
     * tabs which are getting hovered with the mouse are getting visual highlighted (#24)
	 * use white sound icons instead of black ones (#26)
   * Linux theme:
     * tabs which are getting hovered with the mouse are getting visual highlighted (#24)
	 * fixed: unwanted white bar at bottom of window (#16)
   * Dark theme:
     * make background of the favicons transparent instead of white (#18)
	 * use white close icon and white sound icons instead of black ones (#26)
	 * add blue left border to pinned tabs (#32)
	 * fixed: unwanted white bar at bottom of window (#16)
	 * internal: port to Basic template
   * Light theme:
   	 * add blue left border to pinned tabs (#32)
	 * fixed: unwanted white bar at bottom of window (#16)
	 * internal: port to Basic template
 * fixed: toolbar context menu was damaged (#27)
 * fixed: browser.tabs.animated was just disabled one time instead of always
 * heavily refactoring of the code base


***


### v0.4.0, 2016-03-15
 * added possibility to hide/show the tab sidebar manually at any time with a hotkey (customizable) (#6)
 * migrated the add-on to package.json & JPM (#7)
 * added an icon (#3)
 * removed broken group and multiselect features (#10, #12)
 * heavily refactoring of the code base


***


### v0.3.2, 2016-03-01
 * published on Mozilla's Add-on page for auto updates and user friendly installing (#5)
 * fixed: settings were not persistent (#1)
 * added credits
 * refactoring of the code base


***


### v0.3.0, 2015-05-24
 * license updated to MPL 2.0 (from MPL 1.1)
 * tabs are getting hidden in fullscreen finally (toggleable)
 * fixed: style problem on Windows
