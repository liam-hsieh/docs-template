This is a testing page that we prepare to move all markdown files to this page as an official site of documentation.

How to add link:
```
[example link](Section1/test-in-section1.md)
```

[example link](Section1/test-in-section1.md)


Since Github doesn't officially support mermaid for Github page, we applied a workaround to enable a class for <div> could be rendered correctly via external js. 
```
<div class="mermaid">
  flowchart  LR;
    Start-->|scenario,area| M1[Model I] 
    M1-->F1{feasible?}
    F1-->|no| End
    F1-->|yes| M2[Model II]
    M2-->M3[Model III]
    M3-->Complete
</div>
```

<div class="mermaid">
  flowchart  LR;
    Start-->|scenario,area| M1[Model I] 
    M1-->F1{feasible?}
    F1-->|no| End
    F1-->|yes| M2[Model II]
    M2-->M3[Model III]
    M3-->Complete
</div>
