import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      theme: ThemeData.light(), // Используем лёгкую тему для совместимости
      home: Scaffold(
        appBar: AppBar(
          title: Text('Кнопки Приложение'),
        ),
        body: Center(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: <Widget>[
              RaisedButton(
                onPressed: () {
                  print('Первая кнопка нажата');
                },
                child: Text('Кнопка 1'),
              ),
              SizedBox(height: 20),
              RaisedButton(
                onPressed: () {
                  print('Вторая кнопка нажата');
                },
                child: Text('Кнопка 2'),
              ),
              SizedBox(height: 20),
              RaisedButton(
                onPressed: () {
                  print('Третья кнопка нажата');
                },
                child: Text('Кнопка 3'),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
