import java.awt.event.*;  
import javax.swing.*;  
public class wclc extends JFrame implements ActionListener{  
JTextArea ta;  
JButton b1,b2,b3;  
wclc(){  
    super("Words, Characters and Lines Counter");  
    ta=new JTextArea();  
    ta.setBounds(50,50,300,200);  
      
    b1=new JButton("Word");  
    b1.setBounds(10,300,100,30);  
      
    b2=new JButton("Character");  
    b2.setBounds(150,300,100,30); 
    
    b3=new JButton("Line");
    b3.setBounds(290,300,100,30);
    
      
    b1.addActionListener(this);  
    b2.addActionListener(this); 
    b3.addActionListener(this);
    add(b1);add(b2);add(b3);add(ta);  
    setSize(400,400);  
    setLayout(null);  
    setVisible(true);  
}  
public void actionPerformed(ActionEvent e){  
    String text=ta.getText();  
    if(e.getSource()==b1){  
        String words[]=text.split("\\s");  
        JOptionPane.showMessageDialog(this,"Total words: "+words.length);  
    }  
    if(e.getSource()==b2){  
        JOptionPane.showMessageDialog(this,"Total Characters with spaces: "+text.length());  
    }  
    if(e.getSource()==b3){
    	String s[]=text.split("\\n");
    	JOptionPane.showMessageDialog(this,"Total Lines: "+s.length);
    }
}  
public static void main(String[] args) {  
    new wclc();  
}  
}  
