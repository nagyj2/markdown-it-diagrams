# markdown-it-diagrams
Diagrams renderer for [markdown-it](https://github.com/markdown-it/markdown-it), using [svgbob](https://github.com/ivanceras/svgbob), and [mermaidjs](https://github.com/knsv/mermaid).

Example code
~~~
``` bob 
     .---.
    /-o-/--
 .-/ / /->
( *  \/
 '-.  \
    \ /
     '
```
~~~

~~~
``` mermaid 
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
~~~

<image src="data:image/svg+xml,%3Csvg%20id%3D%22mermaid-1552672429889%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20height%3D%22100%25%22%20viewBox%3D%220%200%20166.71875%20289%22%20style%3D%22max-width%3A166.71875px%3B%22%3E%3Cstyle%3E%23mermaid-1552672429889%20.label%7Bfont-family%3Atrebuchet%20ms%2Cverdana%2Carial%3Bcolor%3A%23333%7D%23mermaid-1552672429889%20.node%20circle%2C%23mermaid-1552672429889%20.node%20ellipse%2C%23mermaid-1552672429889%20.node%20polygon%2C%23mermaid-1552672429889%20.node%20rect%7Bfill%3A%23ececff%3Bstroke%3A%239370db%3Bstroke-width%3A1px%7D%23mermaid-1552672429889%20.node.clickable%7Bcursor%3Apointer%7D%23mermaid-1552672429889%20.arrowheadPath%7Bfill%3A%23333%7D%23mermaid-1552672429889%20.edgePath%20.path%7Bstroke%3A%23333%3Bstroke-width%3A1.5px%7D%23mermaid-1552672429889%20.edgeLabel%7Bbackground-color%3A%23e8e8e8%7D%23mermaid-1552672429889%20.cluster%20rect%7Bfill%3A%23ffffde!important%3Bstroke%3A%23aa3!important%3Bstroke-width%3A1px!important%7D%23mermaid-1552672429889%20.cluster%20text%7Bfill%3A%23333%7D%23mermaid-1552672429889%20div.mermaidTooltip%7Bposition%3Aabsolute%3Btext-align%3Acenter%3Bmax-width%3A200px%3Bpadding%3A2px%3Bfont-family%3Atrebuchet%20ms%2Cverdana%2Carial%3Bfont-size%3A12px%3Bbackground%3A%23ffffde%3Bborder%3A1px%20solid%20%23aa3%3Bborder-radius%3A2px%3Bpointer-events%3Anone%3Bz-index%3A100%7D%23mermaid-1552672429889%20.actor%7Bstroke%3A%23ccf%3Bfill%3A%23ececff%7D%23mermaid-1552672429889%20text.actor%7Bfill%3A%23000%3Bstroke%3Anone%7D%23mermaid-1552672429889%20.actor-line%7Bstroke%3Agrey%7D%23mermaid-1552672429889%20.messageLine0%7Bmarker-end%3A%22url(%23arrowhead)%22%7D%23mermaid-1552672429889%20.messageLine0%2C%23mermaid-1552672429889%20.messageLine1%7Bstroke-width%3A1.5%3Bstroke-dasharray%3A%222%202%22%3Bstroke%3A%23333%7D%23mermaid-1552672429889%20%23arrowhead%7Bfill%3A%23333%7D%23mermaid-1552672429889%20%23crosshead%20path%7Bfill%3A%23333!important%3Bstroke%3A%23333!important%7D%23mermaid-1552672429889%20.messageText%7Bfill%3A%23333%3Bstroke%3Anone%7D%23mermaid-1552672429889%20.labelBox%7Bstroke%3A%23ccf%3Bfill%3A%23ececff%7D%23mermaid-1552672429889%20.labelText%2C%23mermaid-1552672429889%20.loopText%7Bfill%3A%23000%3Bstroke%3Anone%7D%23mermaid-1552672429889%20.loopLine%7Bstroke-width%3A2%3Bstroke-dasharray%3A%222%202%22%3Bmarker-end%3A%22url(%23arrowhead)%22%3Bstroke%3A%23ccf%7D%23mermaid-1552672429889%20.note%7Bstroke%3A%23aa3%3Bfill%3A%23fff5ad%7D%23mermaid-1552672429889%20.noteText%7Bfill%3A%23000%3Bstroke%3Anone%3Bfont-family%3Atrebuchet%20ms%2Cverdana%2Carial%3Bfont-size%3A14px%7D%23mermaid-1552672429889%20.section%7Bstroke%3Anone%3Bopacity%3A.2%7D%23mermaid-1552672429889%20.section0%7Bfill%3Argba(102%2C102%2C255%2C.49)%7D%23mermaid-1552672429889%20.section2%7Bfill%3A%23fff400%7D%23mermaid-1552672429889%20.section1%2C%23mermaid-1552672429889%20.section3%7Bfill%3A%23fff%3Bopacity%3A.2%7D%23mermaid-1552672429889%20.sectionTitle0%2C%23mermaid-1552672429889%20.sectionTitle1%2C%23mermaid-1552672429889%20.sectionTitle2%2C%23mermaid-1552672429889%20.sectionTitle3%7Bfill%3A%23333%7D%23mermaid-1552672429889%20.sectionTitle%7Btext-anchor%3Astart%3Bfont-size%3A11px%3Btext-height%3A14px%7D%23mermaid-1552672429889%20.grid%20.tick%7Bstroke%3A%23d3d3d3%3Bopacity%3A.3%3Bshape-rendering%3AcrispEdges%7D%23mermaid-1552672429889%20.grid%20path%7Bstroke-width%3A0%7D%23mermaid-1552672429889%20.today%7Bfill%3Anone%3Bstroke%3Ared%3Bstroke-width%3A2px%7D%23mermaid-1552672429889%20.task%7Bstroke-width%3A2%7D%23mermaid-1552672429889%20.taskText%7Btext-anchor%3Amiddle%3Bfont-size%3A11px%7D%23mermaid-1552672429889%20.taskTextOutsideRight%7Bfill%3A%23000%3Btext-anchor%3Astart%3Bfont-size%3A11px%7D%23mermaid-1552672429889%20.taskTextOutsideLeft%7Bfill%3A%23000%3Btext-anchor%3Aend%3Bfont-size%3A11px%7D%23mermaid-1552672429889%20.taskText0%2C%23mermaid-1552672429889%20.taskText1%2C%23mermaid-1552672429889%20.taskText2%2C%23mermaid-1552672429889%20.taskText3%7Bfill%3A%23fff%7D%23mermaid-1552672429889%20.task0%2C%23mermaid-1552672429889%20.task1%2C%23mermaid-1552672429889%20.task2%2C%23mermaid-1552672429889%20.task3%7Bfill%3A%238a90dd%3Bstroke%3A%23534fbc%7D%23mermaid-1552672429889%20.taskTextOutside0%2C%23mermaid-1552672429889%20.taskTextOutside1%2C%23mermaid-1552672429889%20.taskTextOutside2%2C%23mermaid-1552672429889%20.taskTextOutside3%7Bfill%3A%23000%7D%23mermaid-1552672429889%20.active0%2C%23mermaid-1552672429889%20.active1%2C%23mermaid-1552672429889%20.active2%2C%23mermaid-1552672429889%20.active3%7Bfill%3A%23bfc7ff%3Bstroke%3A%23534fbc%7D%23mermaid-1552672429889%20.activeText0%2C%23mermaid-1552672429889%20.activeText1%2C%23mermaid-1552672429889%20.activeText2%2C%23mermaid-1552672429889%20.activeText3%7Bfill%3A%23000!important%7D%23mermaid-1552672429889%20.done0%2C%23mermaid-1552672429889%20.done1%2C%23mermaid-1552672429889%20.done2%2C%23mermaid-1552672429889%20.done3%7Bstroke%3Agrey%3Bfill%3A%23d3d3d3%3Bstroke-width%3A2%7D%23mermaid-1552672429889%20.doneText0%2C%23mermaid-1552672429889%20.doneText1%2C%23mermaid-1552672429889%20.doneText2%2C%23mermaid-1552672429889%20.doneText3%7Bfill%3A%23000!important%7D%23mermaid-1552672429889%20.crit0%2C%23mermaid-1552672429889%20.crit1%2C%23mermaid-1552672429889%20.crit2%2C%23mermaid-1552672429889%20.crit3%7Bstroke%3A%23f88%3Bfill%3Ared%3Bstroke-width%3A2%7D%23mermaid-1552672429889%20.activeCrit0%2C%23mermaid-1552672429889%20.activeCrit1%2C%23mermaid-1552672429889%20.activeCrit2%2C%23mermaid-1552672429889%20.activeCrit3%7Bstroke%3A%23f88%3Bfill%3A%23bfc7ff%3Bstroke-width%3A2%7D%23mermaid-1552672429889%20.doneCrit0%2C%23mermaid-1552672429889%20.doneCrit1%2C%23mermaid-1552672429889%20.doneCrit2%2C%23mermaid-1552672429889%20.doneCrit3%7Bstroke%3A%23f88%3Bfill%3A%23d3d3d3%3Bstroke-width%3A2%3Bcursor%3Apointer%3Bshape-rendering%3AcrispEdges%7D%23mermaid-1552672429889%20.activeCritText0%2C%23mermaid-1552672429889%20.activeCritText1%2C%23mermaid-1552672429889%20.activeCritText2%2C%23mermaid-1552672429889%20.activeCritText3%2C%23mermaid-1552672429889%20.doneCritText0%2C%23mermaid-1552672429889%20.doneCritText1%2C%23mermaid-1552672429889%20.doneCritText2%2C%23mermaid-1552672429889%20.doneCritText3%7Bfill%3A%23000!important%7D%23mermaid-1552672429889%20.titleText%7Btext-anchor%3Amiddle%3Bfont-size%3A18px%3Bfill%3A%23000%7D%23mermaid-1552672429889%20g.classGroup%20text%7Bfill%3A%239370db%3Bstroke%3Anone%3Bfont-family%3Atrebuchet%20ms%2Cverdana%2Carial%3Bfont-size%3A10px%7D%23mermaid-1552672429889%20g.classGroup%20rect%7Bfill%3A%23ececff%3Bstroke%3A%239370db%7D%23mermaid-1552672429889%20g.classGroup%20line%7Bstroke%3A%239370db%3Bstroke-width%3A1%7D%23mermaid-1552672429889%20.classLabel%20.box%7Bstroke%3Anone%3Bstroke-width%3A0%3Bfill%3A%23ececff%3Bopacity%3A.5%7D%23mermaid-1552672429889%20.classLabel%20.label%7Bfill%3A%239370db%3Bfont-size%3A10px%7D%23mermaid-1552672429889%20.relation%7Bstroke%3A%239370db%3Bstroke-width%3A1%3Bfill%3Anone%7D%23mermaid-1552672429889%20%23compositionEnd%2C%23mermaid-1552672429889%20%23compositionStart%7Bfill%3A%239370db%3Bstroke%3A%239370db%3Bstroke-width%3A1%7D%23mermaid-1552672429889%20%23aggregationEnd%2C%23mermaid-1552672429889%20%23aggregationStart%7Bfill%3A%23ececff%3Bstroke%3A%239370db%3Bstroke-width%3A1%7D%23mermaid-1552672429889%20%23dependencyEnd%2C%23mermaid-1552672429889%20%23dependencyStart%2C%23mermaid-1552672429889%20%23extensionEnd%2C%23mermaid-1552672429889%20%23extensionStart%7Bfill%3A%239370db%3Bstroke%3A%239370db%3Bstroke-width%3A1%7D%23mermaid-1552672429889%20.branch-label%2C%23mermaid-1552672429889%20.commit-id%2C%23mermaid-1552672429889%20.commit-msg%7Bfill%3A%23d3d3d3%3Bcolor%3A%23d3d3d3%7D%3C%2Fstyle%3E%3Cstyle%3E%23mermaid-1552672429889%20%7B%0A%20%20%20%20color%3A%20rgb(51%2C%2051%2C%2051)%3B%0A%20%20%20%20font%3A%20normal%20normal%20400%20normal%2013.6px%20%2F%2023.12px%20Consolas%2C%20%22Liberation%20Mono%22%2C%20Menlo%2C%20Courier%2C%20monospace%3B%0A%20%20%7D%3C%2Fstyle%3E%3Cg%3E%3Cg%20class%3D%22output%22%3E%3Cg%20class%3D%22clusters%22%3E%3C%2Fg%3E%3Cg%20class%3D%22edgePaths%22%3E%3Cg%20class%3D%22edgePath%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cpath%20class%3D%22path%22%20d%3D%22M59.1796875%2C58.329012961116646L34.1796875%2C88L34.1796875%2C113%22%20marker-end%3D%22url(%23arrowhead14)%22%20style%3D%22fill%3Anone%22%3E%3C%2Fpath%3E%3Cdefs%3E%3Cmarker%20id%3D%22arrowhead14%22%20viewBox%3D%220%200%2010%2010%22%20refX%3D%229%22%20refY%3D%225%22%20markerUnits%3D%22strokeWidth%22%20markerWidth%3D%228%22%20markerHeight%3D%226%22%20orient%3D%22auto%22%3E%3Cpath%20d%3D%22M%200%200%20L%2010%205%20L%200%2010%20z%22%20class%3D%22arrowheadPath%22%20style%3D%22stroke-width%3A%201%3B%20stroke-dasharray%3A%201%2C%200%3B%22%3E%3C%2Fpath%3E%3C%2Fmarker%3E%3C%2Fdefs%3E%3C%2Fg%3E%3Cg%20class%3D%22edgePath%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cpath%20class%3D%22path%22%20d%3D%22M87.5390625%2C58.329012961116646L112.5390625%2C88L112.5390625%2C113%22%20marker-end%3D%22url(%23arrowhead15)%22%20style%3D%22fill%3Anone%22%3E%3C%2Fpath%3E%3Cdefs%3E%3Cmarker%20id%3D%22arrowhead15%22%20viewBox%3D%220%200%2010%2010%22%20refX%3D%229%22%20refY%3D%225%22%20markerUnits%3D%22strokeWidth%22%20markerWidth%3D%228%22%20markerHeight%3D%226%22%20orient%3D%22auto%22%3E%3Cpath%20d%3D%22M%200%200%20L%2010%205%20L%200%2010%20z%22%20class%3D%22arrowheadPath%22%20style%3D%22stroke-width%3A%201%3B%20stroke-dasharray%3A%201%2C%200%3B%22%3E%3C%2Fpath%3E%3C%2Fmarker%3E%3C%2Fdefs%3E%3C%2Fg%3E%3Cg%20class%3D%22edgePath%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cpath%20class%3D%22path%22%20d%3D%22M34.1796875%2C156L34.1796875%2C181L59.1796875%2C210.67098703888334%22%20marker-end%3D%22url(%23arrowhead16)%22%20style%3D%22fill%3Anone%22%3E%3C%2Fpath%3E%3Cdefs%3E%3Cmarker%20id%3D%22arrowhead16%22%20viewBox%3D%220%200%2010%2010%22%20refX%3D%229%22%20refY%3D%225%22%20markerUnits%3D%22strokeWidth%22%20markerWidth%3D%228%22%20markerHeight%3D%226%22%20orient%3D%22auto%22%3E%3Cpath%20d%3D%22M%200%200%20L%2010%205%20L%200%2010%20z%22%20class%3D%22arrowheadPath%22%20style%3D%22stroke-width%3A%201%3B%20stroke-dasharray%3A%201%2C%200%3B%22%3E%3C%2Fpath%3E%3C%2Fmarker%3E%3C%2Fdefs%3E%3C%2Fg%3E%3Cg%20class%3D%22edgePath%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cpath%20class%3D%22path%22%20d%3D%22M112.5390625%2C156L112.5390625%2C181L87.5390625%2C210.67098703888334%22%20marker-end%3D%22url(%23arrowhead17)%22%20style%3D%22fill%3Anone%22%3E%3C%2Fpath%3E%3Cdefs%3E%3Cmarker%20id%3D%22arrowhead17%22%20viewBox%3D%220%200%2010%2010%22%20refX%3D%229%22%20refY%3D%225%22%20markerUnits%3D%22strokeWidth%22%20markerWidth%3D%228%22%20markerHeight%3D%226%22%20orient%3D%22auto%22%3E%3Cpath%20d%3D%22M%200%200%20L%2010%205%20L%200%2010%20z%22%20class%3D%22arrowheadPath%22%20style%3D%22stroke-width%3A%201%3B%20stroke-dasharray%3A%201%2C%200%3B%22%3E%3C%2Fpath%3E%3C%2Fmarker%3E%3C%2Fdefs%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22edgeLabels%22%3E%3Cg%20class%3D%22edgeLabel%22%20transform%3D%22%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cg%20transform%3D%22translate(0%2C0)%22%20class%3D%22label%22%3E%3CforeignObject%20width%3D%220%22%20height%3D%220%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3E%3Cspan%20class%3D%22edgeLabel%22%3E%3C%2Fspan%3E%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22edgeLabel%22%20transform%3D%22%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cg%20transform%3D%22translate(0%2C0)%22%20class%3D%22label%22%3E%3CforeignObject%20width%3D%220%22%20height%3D%220%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3E%3Cspan%20class%3D%22edgeLabel%22%3E%3C%2Fspan%3E%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22edgeLabel%22%20transform%3D%22%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cg%20transform%3D%22translate(0%2C0)%22%20class%3D%22label%22%3E%3CforeignObject%20width%3D%220%22%20height%3D%220%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3E%3Cspan%20class%3D%22edgeLabel%22%3E%3C%2Fspan%3E%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22edgeLabel%22%20transform%3D%22%22%20style%3D%22opacity%3A%201%3B%22%3E%3Cg%20transform%3D%22translate(0%2C0)%22%20class%3D%22label%22%3E%3CforeignObject%20width%3D%220%22%20height%3D%220%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3E%3Cspan%20class%3D%22edgeLabel%22%3E%3C%2Fspan%3E%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22nodes%22%3E%3Cg%20class%3D%22node%22%20id%3D%22A%22%20transform%3D%22translate(73.359375%2C41.5)%22%20style%3D%22opacity%3A%201%3B%22%3E%3Crect%20rx%3D%220%22%20ry%3D%220%22%20x%3D%22-14.1796875%22%20y%3D%22-21.5%22%20width%3D%2228.359375%22%20height%3D%2243%22%3E%3C%2Frect%3E%3Cg%20class%3D%22label%22%20transform%3D%22translate(0%2C0)%22%3E%3Cg%20transform%3D%22translate(-4.1796875%2C-11.5)%22%3E%3CforeignObject%20width%3D%228.359375%22%20height%3D%2223%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3EA%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22node%22%20id%3D%22B%22%20transform%3D%22translate(34.1796875%2C134.5)%22%20style%3D%22opacity%3A%201%3B%22%3E%3Crect%20rx%3D%220%22%20ry%3D%220%22%20x%3D%22-14.1796875%22%20y%3D%22-21.5%22%20width%3D%2228.359375%22%20height%3D%2243%22%3E%3C%2Frect%3E%3Cg%20class%3D%22label%22%20transform%3D%22translate(0%2C0)%22%3E%3Cg%20transform%3D%22translate(-4.1796875%2C-11.5)%22%3E%3CforeignObject%20width%3D%228.359375%22%20height%3D%2223%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3EB%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22node%22%20id%3D%22C%22%20transform%3D%22translate(112.5390625%2C134.5)%22%20style%3D%22opacity%3A%201%3B%22%3E%3Crect%20rx%3D%220%22%20ry%3D%220%22%20x%3D%22-14.1796875%22%20y%3D%22-21.5%22%20width%3D%2228.359375%22%20height%3D%2243%22%3E%3C%2Frect%3E%3Cg%20class%3D%22label%22%20transform%3D%22translate(0%2C0)%22%3E%3Cg%20transform%3D%22translate(-4.1796875%2C-11.5)%22%3E%3CforeignObject%20width%3D%228.359375%22%20height%3D%2223%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3EC%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3Cg%20class%3D%22node%22%20id%3D%22D%22%20transform%3D%22translate(73.359375%2C227.5)%22%20style%3D%22opacity%3A%201%3B%22%3E%3Crect%20rx%3D%220%22%20ry%3D%220%22%20x%3D%22-14.1796875%22%20y%3D%22-21.5%22%20width%3D%2228.359375%22%20height%3D%2243%22%3E%3C%2Frect%3E%3Cg%20class%3D%22label%22%20transform%3D%22translate(0%2C0)%22%3E%3Cg%20transform%3D%22translate(-4.1796875%2C-11.5)%22%3E%3CforeignObject%20width%3D%228.359375%22%20height%3D%2223%22%3E%3Cdiv%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1999%2Fxhtml%22%20style%3D%22display%3A%20inline-block%3B%20white-space%3A%20nowrap%3B%22%3ED%3C%2Fdiv%3E%3C%2FforeignObject%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E">
