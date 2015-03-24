# CSE360ProjectV1

package simplelogin;


import java.awt.Color;

import javax.swing.JButton;
import javax.swing.JFrame; //library
import javax.swing.JLabel;
import javax.swing.JPasswordField;
import javax.swing.JTextField;

public class Gui {

	JFrame frame; //frame
	JTextField field;
	JPasswordField p;
	JLabel l;
	JButton b, e;
	
	Gui () {
		
		frame = new JFrame ("Login Screen ");
		frame.setSize(500,200);
		//frame.getContentPane().setBackground(Color.black);
		frame.setLocation(300,200);
		frame.setLayout(null);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		
		l = new JLabel ("User Name");
		l.setLocation(50,10);
		l.setSize(l.getPreferredSize());
		frame.add(l);
		
		field = new JTextField();
		field.setColumns(25);
		field.setSize(field.getPreferredSize());
	
		field.setLocation(150, 10);
		field.setToolTipText("Enter User Name");
		frame.add(field);
		
		l = new JLabel ("Password");
		l.setLocation(50,40);
		l.setSize(l.getPreferredSize());
		frame.add(l);
		
		p = new JPasswordField();
		p.setColumns(25);
		p.setSize(p.getPreferredSize());
	
		p.setLocation(150, 40);
		p.setToolTipText("Enter Password");
		frame.add(p);
		
		b = new JButton("Login");
		b.setSize(b.getPreferredSize());
		b.setLocation(150,80);
		frame.add(b);
		
		e = new JButton("Emergency");
		e.setSize(e.getPreferredSize());
		e.setLocation(300,80);
		frame.add(e);
		
		frame.setVisible(true);
		
		
	}
	
	public static void main(String args[]){
		new Gui ();
	}
	
	
}
