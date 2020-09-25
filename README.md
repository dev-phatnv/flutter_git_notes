# flutter_git_notes
1. SafeArea
2. Expanded (flex, rest space) <br/>
  Expanded(
    flex: 2,
    child: Container()
  );
3. Wrap (runs out of space, it just wraps to the next line) <br/>
  Wrap(
    direction: Axis.verticle,
    children: [
      MyWidget(),
    ],
    alignment: WrapAlignment.end,
    spacing: 10.0,
    runSpacing: 20.0
  );
4. AnimatedContainer <br/>
5. Opacity (Widget to disappear but still take up space || blending stacks) <br/>
  Opacity(
    opacity: 0.0,
    child: MyWidget(Colors.green),
  );

  Stack(
    children: [
      MyImageWidget(),
      Opacity(
        opacity: 0.25,
        child: MyGradientWidget(),
      ),
    ]
  );
  
  
  Stack(
    children: [
      MyImageWidget(),
      AnimatedOpacity(
        opacity: _myOpacity,
        duration: _myDuration,
        child: MyGradientWidget(),
      ),
    ]
  );
  
  6. FutureBuilder
  7. FadeTransition
  8. FloatingActionButton
  9. PageView
  10. Table (process tab2 => lecture 2)
  11. SliverAppBar
  12. SliverList & SliverGrid
  14. FadeInImage
  15. StreamBuilder
  16. InheritedModel
  
