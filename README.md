[![Published on Vaadin  Directory](https://img.shields.io/badge/Vaadin%20Directory-published-00b4f0.svg)](https://vaadin.com/directory/component/history)
[![Stars on Vaadin Directory](https://img.shields.io/vaadin-directory/star/history.svg)](https://vaadin.com/directory/component/history)

# HistoryExtension

A HTML 5 history wrapper for Vaadin server-side. 

Example usage:

    HistoryExtension history = HistoryExtension.extend(myUI, myPopStateListener);
    
    // init app state
    history.replaceState(getCurrentAppState(), getPage().getLocation().toString());
    
    addComponent(new Button("next step", new ClickListener() {
      public void buttonClick(final ClickEvent event) {
        history.pushState(getNextAppState(), "nextStep.html");
      }
    }));

For complete demos, check out [simpledemo][sdlink], [tabledemo][tdlink] and [navigatordemo][ndlink]
[sdlink]: https://github.com/wolfie/HistoryExtension/tree/master/src/test/java/com/github/wolfie/history/simpledemo
[tdlink]: https://github.com/wolfie/HistoryExtension/tree/master/src/test/java/com/github/wolfie/history/tabledemo
[ndlink]: https://github.com/wolfie/HistoryExtension/tree/master/src/test/java/com/github/wolfie/history/navigatordemo
