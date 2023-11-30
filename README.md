# LOGIN-PAGE
class
 
LoginPage
 
extends
 
StatelessWidget
 
{
  const LoginPage({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Login'),
      ),
      body: Column(
        children: [
          // Email Text Field
          TextField(
            decoration: InputDecoration(
              labelText: 'Email Address',
              border: OutlineInputBorder(),
            ),
          ),

          // Password Text Field
          TextField(
            obscureText: true, // Hides password characters
            decoration: InputDecoration(
              labelText: 'Password',
              border: OutlineInputBorder(),
            ),
          ),

          // Login Button
          SizedBox(height: 20),
          ElevatedButton(
            onPressed: () {},
            child: Text('Login'),
          ),

          // Forgot Password Link
          SizedBox(height: 20),
          TextButton(
            onPressed: () {},
            child: Text('Forgot Password?'),
          ),
        ],
      ),
    );
  }
}
import
 
'package:flutter/material.dart';
import
 
'package:login_app/LoginPage.dart';

void main() {
  runApp(MyApp());
}

class
 
MyApp
 
extends
 
StatelessWidget
 
{
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Login App',
      home: LoginPage(),
    );
  }
}
