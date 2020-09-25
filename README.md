# flutter_git_notes
1. SafeArea
2. Expanded (flex, rest space)
  Expanded(
    flex: 2,
    child: Container()
  );
3. Wrap (runs out of space, it just wraps to the next line)
  Wrap(
    direction: Axis.verticle,
    children: [
      MyWidget(),
    ],
    alignment: WrapAlignment.end,
    spacing: 10.0,
    runSpacing: 20.0
  );
4. AnimatedContainer
5. Opacity (Widget to disappear but still take up space || blending stacks)
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
  
