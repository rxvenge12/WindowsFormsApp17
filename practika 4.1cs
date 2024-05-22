using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp11
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }
        private void textBox1_TextChanged(object sender, EventArgs e)
        {
            
        }

        private void countButton_Click(object sender, EventArgs e)
        {
            string inputText = textBox1.Text;
            char letterToCheck = textBox2.Text.ToLower()[0]; 
            int wordCount = CountWordsEndingWithLetter(inputText, letterToCheck);
            label1.Text = $"Количество слов, оканчивающихся на '{letterToCheck}': {wordCount}";
        }

        private int CountWordsEndingWithLetter(string inputText, char letter)
        {
            int count = 0;

            
            string[] words = inputText.Split(new char[] { ',', '.' }, StringSplitOptions.RemoveEmptyEntries);

            foreach (string word in words)
            {
                
                if (word.Trim().ToLower().EndsWith(letter.ToString()))
                {
                    count++;
                }
            }

            return count;
        }
    }
}
    