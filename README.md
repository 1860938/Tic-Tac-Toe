# README
Creation of a README
Tic Tac Toe

This application, 
this should let the user play Tic Tac Toe in the console, I utilized technologies learned through the whole year as well as learning new teniques such as shorthand for loops as well as the integration of char. Being gone for a week really held back my progress, I initially wanted to create a tower defence game however, my progress was slow and so I decided to just create a TicTacToe game, these proved to be too difficult and I was left with 2 unfinished games. Although I would like to have one good functioning game, it wasnt very plausible because of my poor descisions

Application,
All one would need to do is to open the files in eclipse or any other java IDE and the code should run given that it works.

How to use it,
With this application, you can play Tic Tac Toe to your heart's content with a robot.

Credits,
I created this game myself with some logical help from many other people.

##GitHub would not let me push my code


##Tic Tac Toe:
/*import java.util.Scanner;

public class TicTacToe {

	public static void main(String[] args) {
		
		
		String [][] gameBoard = {{' ', '|', ' ', '|', ' '},
							  {'-', '+', '-', '+', '-'},
							  {' ', '|', ' ', '|', ' '},
							  {'-', '+', '-', '+', '-'},
							  {' ', '|', ' ', '|', ' '}
							 
        };
printGameBoard(gameBoard);

Scanner scan = new Scanner(System.in);
System.out.println("Place your piece");
System.out.println();
int pos = scan.nextInt();

	
	public static void printGameBoard (String[][] gameBoard) {
		for(String[] row : gameBoard) {
			for(String c : row) {
				System.out.print(c);
			}
			System.out.println();
		}
	


#Tower Defence
g.setColor(Color.WHITE);
        g.fillRect(300, 0, 100, 300);
        
                g.setColor(Color.RED);
        g.setFont(new Font("Comic Sans", Font.BOLD, 18));
        g.drawString("Health: " + livesCounter, 305, 150);	
        g.drawString("Money Earned: " + scoreCounter, 305, 100);	
        g.drawString("Balloons popped: " + killsCounter, 305, 100);
        g.drawString("Ranger Monkey cost: 200", 600, 200);			
        g.drawLine(600, 50, 400, 50);								
        g.drawString("Towers", 340, 200);						
        g.drawLine(625, 240, 300, 140);	
        g.drawString("Monkey Cost: 100", 300, 200);					
        g.setFont(new Font("Comic Sans", Font.BOLD, 20));		
        g.drawString("Tower", 300, 50);					
						
        
        g.setColor(new Color (0,70, 150));
        int[] xPos = new int[]{0, 64, 118, 251, 298, 344, 396, 416, 437, 459, 460, 498, 542, 600, 600, 568, 535, 509, 490, 481, 456, 414, 345, 287, 227, 98, 0};
        int[] yPos = new int[]{329, 316, 291, 189, 163, 154, 165, 186, 233, 344, 364, 415, 444, 461, 410, 396, 372, 331, 226, 195, 151, 117, 105, 117, 143, 244, 280};
        g.fillPolygon(xPos, yPos, 27);
        

        g.setColor(new Color(60,100,125));
        g.fillArc(550, 105, 100, 100, 90, 180);
        g.setColor(Color.BLUE);
        int[] xCor = new int[]{600, 588, 574, 566, 557, 557, 563, 572, 576, 584, 600};
        int[] yCor = new int[]{459, 464, 462, 453, 454, 448, 438, 435, 422, 414, 415};
        g.fillPolygon(xCor, yCor, 11);
        


                g.setColor(new Color(224, 224, 224));
        g.fillRect(600, 200, 50, 50);
        
               monkeyRanger = new MonkeyRanger(new Coordinate(600, 300));
        monkeyranger.draw(g);
        
                g.setColor(new Color(200, 200, 200));
        g.fillRect(600, 200, 100, 50);
        
   
    Monkey monkey = new Monkey(new Coordinate(350, 250));
        monkey.draw(g);
        
   
        if(newMonkeyRanger != null)
        	newMonkeyRanger.draw(g);

        if(Monkey != null)
        	newMonkey.draw(g);
        
        ImageLoader loader = ImageLoader.getLoader();	
		Image endGame = loader.getImage("/*to be implemented*/"); 
    	
        if(livesCounter <= 0)										
        	g.drawImage(endGame, 0, 0, null);						

		if(killsCounter >= 10)										
		{	g.setFont(new Font("Comic Sans", Font.BOLD, 100));		
        	g.drawString("You Win", 100, 200);					
		}
		 
    }
    

    public void generateEnemies(){
    
  

 	    

    public void placeRangerMonkey(){


  
    	Coordinate mouseLocation = new Coordinate(gamePanel.mouseX, gamePanel.mouseY);
    	
 
    	if(gamePanel.mouseX > 600 && gamePanel.mouseX < 700 && 
    		gamePanel.mouseY > 200 && gamePanel.mouseY < 300 && 
    		gamePanel.mouseIsPressed && scoreCounter >= 50)
    	{	
	    		placingRangerMonkey = true;
	    		newRangerMonkey = new RangerMonkey(mouseLocation);
    	}    
    	else if(gamePanel.mouseX > 0 && gamePanel.mouseX < 600 && 
        	gamePanel.mouseY > 0 && gamePanel.mouseY < 600 && 
        	gamePanel.mouseIsPressed && placingRangerMonkey
        	&& line.distanceToPath(gamePanel.mouseX, gamePanel.mouseY) > 60)
    	{	
	    		newRangerMonkey.setPosition(mouseLocation);
	    		towers.add(new RangerMonkey(mouseLocation));
	    		scoreCounter -= 100;
	    		newRangerMonkey = null;
	    		placingRangerMonkey= false;	
    	}
    	
    	if(newRangerMonkey != null)
    	{
    		newRangerMonkey.setPosition(mouseLocation);
    	}	
    }
    

    public void placeMonkeys()
    {

    	Coordinate mouseLocation = new Coordinate(gamePanel.mouseX, gamePanel.mouseY);
    	
  
    	if(gamePanel.mouseX > 600 && gamePanel.mouseX < 700 && 
    		gamePanel.mouseY > 400 && gamePanel.mouseY < 500 && 
    		gamePanel.mouseIsPressed && scoreCounter >= 200)
    	{	
	    		placingMonkeys = true;
	    		newMonkeys = new Monkeys(mouseLocation);
    	}    
    	else if(gamePanel.mouseX > 0 && gamePanel.mouseX < 600 && 
        	gamePanel.mouseY > 0 && gamePanel.mouseY < 600 && 
        	gamePanel.mouseIsPressed && placingMonkeys
        	&& line.distanceToPath(gamePanel.mouseX, gamePanel.mouseY) > 30)
    	{	
	    		newMonkeys.setPosition(mouseLocation);
	    		towers.add(new Monkeys(mouseLocation));
	    		scoreCounter -= 200;
	    		newMonkeys = null;
	    		placingMonkeys = false;	
    	}
    	
    
    	if(newMonkeys != null)
    	{
    		newMonkeys.setPosition(mouseLocation);
    	}	
    }
*/


