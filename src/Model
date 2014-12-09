
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import javax.swing.JButton;
import javax.swing.JOptionPane;


class ButtonHandler implements ActionListener {
    private final int row, col;
    private final MineGrid grid;

    public ButtonHandler(int x, int y, MineGrid g) {
        row = x;
        col = y;
        grid = g;
    }

    @Override
    public void actionPerformed(ActionEvent event) {
        if(grid.containsMineAt(row, col)) {
            JOptionPane.showMessageDialog(null, "*******************Boom!!! Game Over!!"
                    + "********************");
            System.exit(0);
        } else {
            JButton button = (JButton)event.getSource();
            button.setText(String.valueOf(grid.getInfoAt(row, col)));
        }
    }
}


