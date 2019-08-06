# FirstVueDemo
入门练习
--基础标签
--常用组件
一个现成的vue项目框架，并不成熟，自己拿来分析学习的。

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {
           
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            button1.Visible = false;
            dingwei();
        }

        private void button2_Click(object sender, EventArgs e)
        {
            button2.Visible = false;
            dingwei();
        }

        public void dingwei( ) {
          

            Button[] btnArr = new Button[] { button1, button2, button3, button4, button5, button6};
            List<Button> btnArrShow = new List<Button>();
            foreach (var item in btnArr)
            {
                if (item.Visible)
                {
                    btnArrShow.Add(item);
                }
            }
            for (int i = 0; i < btnArrShow.Count; i++)
            {
                btnArrShow[i].Location = new Point(200*(i%3),100*(i/3));
            }
        }

        private void button6_Click(object sender, EventArgs e)
        {
            button6.Visible = false;
            dingwei();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            button3.Visible = false;
            dingwei();
        }

        private void button4_Click(object sender, EventArgs e)
        {
            button4.Visible = false;
            dingwei();
        }

        private void button5_Click(object sender, EventArgs e)
        {
            button5.Visible = false;
            dingwei();
        }

        private void button7_Click(object sender, EventArgs e)
        {
            Button[] btnArr = new Button[] { button1, button2, button3, button4, button5, button6 };
            foreach (var item in btnArr)
            {
                item.Visible = true;
            }
            dingwei();
        }
    }
}
