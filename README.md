# ROLLER-DICE-GAME
Android App Development(Designed a dice game)
import 'package:flutter/material.dart';

void main() {
  runApp(Demo());
}

class Demo extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.teal,
        appBar: AppBar(
          backgroundColor: Colors.amberAccent,
          title: Text('My Profile',style: TextStyle(color: Colors.black,fontWeight: FontWeight.bold,fontSize: 24.0),),
          centerTitle: true,
        ),
        body:Center(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center,
            children: [
              CircleAvatar(
                radius: 100.0,
                backgroundImage: AssetImage('assets/logo.png'),
              ),
              SizedBox(height: 25.0,),
              Text('Flutter Developer',style: TextStyle(color: Colors.white,fontSize: 25.0),),
              SizedBox(
                width: 200.0,
                child: Divider(
                  color: Colors.black,
                ),
                height: 30.0,
              ),
              Card(
                margin: EdgeInsets.symmetric(vertical:10.0,horizontal:25.0),
//                padding: EdgeInsets.all(10.0),
                color: Colors.white,
                child: Padding(
                    padding: const EdgeInsets.all(4.0),
                    child: ListTile(
                      leading: Icon(Icons.person,size: 40.0,color: Colors.red,),
                      title: Text('Deenadayalan',style: TextStyle(color: Colors.black,fontWeight: FontWeight.bold,fontSize: 28.0),),
                    )
                ),
              ),
              Card(
                margin: EdgeInsets.symmetric(vertical:10.0,horizontal:25.0),
//                padding: EdgeInsets.all(10.0),
                color: Colors.white,
                child: Padding(
                  padding: EdgeInsets.all(4.0),
                  child: ListTile(
                    leading: Icon(Icons.phone,size: 40.0,color:Colors.red,),
                    title: Text('+91-9791654694',style: TextStyle(color: Colors.black,fontWeight: FontWeight.bold,fontSize: 28.0),),
                  ),
                ),
              ),
              Card(
                margin: EdgeInsets.symmetric(vertical:10.0,horizontal:25.0),
//                padding: EdgeInsets.all(10.0),
                color: Colors.white,
                child: Padding(
                  padding: const EdgeInsets.all(4.0),
                  child: ListTile(
                    leading: Icon(Icons.mail,size: 40.0,color: Colors.red,),
                    title: Text('ddvs2499@gmail.com',style: TextStyle(color: Colors.black,fontWeight: FontWeight.bold,fontSize: 28.0),),
                  ),
                ),
              )
            ],
          ),
        ),
      ),
    );
  }
}





