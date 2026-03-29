#pragma once
const int n = 10;
int mas[n]; // глобальний масив


namespace Lz5 {

	using namespace System;
	using namespace System::ComponentModel;
	using namespace System::Collections;
	using namespace System::Windows::Forms;
	using namespace System::Data;
	using namespace System::Drawing;

	/// <summary>
	/// Сводка для MyForm
	/// </summary>
	public ref class MyForm : public System::Windows::Forms::Form
	{
	public:
		MyForm(void)
		{
			InitializeComponent();
			//
			//TODO: добавьте код конструктора
			//
		}

	protected:
		/// <summary>
		/// Освободить все используемые ресурсы.
		/// </summary>
		~MyForm()
		{
			if (components)
			{
				delete components;
			}
		}
	private: System::Windows::Forms::PictureBox^  pictureBox1;
	private: System::Windows::Forms::DataGridView^  dataGridView1;
	private: System::Windows::Forms::DataGridView^  dataGridView2;
	private: System::Windows::Forms::Button^  button1;
	private: System::Windows::Forms::Button^  button2;
	private: System::Windows::Forms::Button^  button3;
	private: System::Windows::Forms::Label^  label1;
	protected: 

	private:
		/// <summary>
		/// Требуется переменная конструктора.
		/// </summary>
		System::ComponentModel::Container ^components;

#pragma region Windows Form Designer generated code
		/// <summary>
		/// Обязательный метод для поддержки конструктора - не изменяйте
		/// содержимое данного метода при помощи редактора кода.
		/// </summary>
		void InitializeComponent(void)
		{
			System::ComponentModel::ComponentResourceManager^  resources = (gcnew System::ComponentModel::ComponentResourceManager(MyForm::typeid));
			this->pictureBox1 = (gcnew System::Windows::Forms::PictureBox());
			this->dataGridView1 = (gcnew System::Windows::Forms::DataGridView());
			this->dataGridView2 = (gcnew System::Windows::Forms::DataGridView());
			this->button1 = (gcnew System::Windows::Forms::Button());
			this->button2 = (gcnew System::Windows::Forms::Button());
			this->button3 = (gcnew System::Windows::Forms::Button());
			this->label1 = (gcnew System::Windows::Forms::Label());
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->pictureBox1))->BeginInit();
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->dataGridView1))->BeginInit();
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->dataGridView2))->BeginInit();
			this->SuspendLayout();
			// 
			// pictureBox1
			// 
			this->pictureBox1->Image = (cli::safe_cast<System::Drawing::Image^  >(resources->GetObject(L"pictureBox1.Image")));
			this->pictureBox1->Location = System::Drawing::Point(12, 12);
			this->pictureBox1->Name = L"pictureBox1";
			this->pictureBox1->Size = System::Drawing::Size(589, 50);
			this->pictureBox1->SizeMode = System::Windows::Forms::PictureBoxSizeMode::StretchImage;
			this->pictureBox1->TabIndex = 0;
			this->pictureBox1->TabStop = false;
			// 
			// dataGridView1
			// 
			this->dataGridView1->ColumnHeadersHeightSizeMode = System::Windows::Forms::DataGridViewColumnHeadersHeightSizeMode::AutoSize;
			this->dataGridView1->Location = System::Drawing::Point(39, 106);
			this->dataGridView1->Name = L"dataGridView1";
			this->dataGridView1->Size = System::Drawing::Size(223, 227);
			this->dataGridView1->TabIndex = 1;
			// 
			// dataGridView2
			// 
			this->dataGridView2->ColumnHeadersHeightSizeMode = System::Windows::Forms::DataGridViewColumnHeadersHeightSizeMode::AutoSize;
			this->dataGridView2->Location = System::Drawing::Point(350, 106);
			this->dataGridView2->Name = L"dataGridView2";
			this->dataGridView2->Size = System::Drawing::Size(226, 227);
			this->dataGridView2->TabIndex = 2;
			// 
			// button1
			// 
			this->button1->Location = System::Drawing::Point(109, 356);
			this->button1->Name = L"button1";
			this->button1->Size = System::Drawing::Size(75, 23);
			this->button1->TabIndex = 3;
			this->button1->Text = L"Заповнити";
			this->button1->UseVisualStyleBackColor = true;
			this->button1->Click += gcnew System::EventHandler(this, &MyForm::button1_Click);
			// 
			// button2
			// 
			this->button2->Location = System::Drawing::Point(419, 356);
			this->button2->Name = L"button2";
			this->button2->Size = System::Drawing::Size(75, 23);
			this->button2->TabIndex = 4;
			this->button2->Text = L"Сортувати";
			this->button2->UseVisualStyleBackColor = true;
			this->button2->Click += gcnew System::EventHandler(this, &MyForm::button2_Click);
			// 
			// button3
			// 
			this->button3->Location = System::Drawing::Point(222, 395);
			this->button3->Name = L"button3";
			this->button3->Size = System::Drawing::Size(177, 23);
			this->button3->TabIndex = 5;
			this->button3->Text = L"Найбільший елемент";
			this->button3->UseVisualStyleBackColor = true;
			this->button3->Click += gcnew System::EventHandler(this, &MyForm::button3_Click);
			// 
			// label1
			// 
			this->label1->AutoSize = true;
			this->label1->Location = System::Drawing::Point(242, 431);
			this->label1->Name = L"label1";
			this->label1->Size = System::Drawing::Size(0, 13);
			this->label1->TabIndex = 6;
			// 
			// MyForm
			// 
			this->AutoScaleDimensions = System::Drawing::SizeF(6, 13);
			this->AutoScaleMode = System::Windows::Forms::AutoScaleMode::Font;
			this->ClientSize = System::Drawing::Size(624, 464);
			this->Controls->Add(this->label1);
			this->Controls->Add(this->button3);
			this->Controls->Add(this->button2);
			this->Controls->Add(this->button1);
			this->Controls->Add(this->dataGridView2);
			this->Controls->Add(this->dataGridView1);
			this->Controls->Add(this->pictureBox1);
			this->Name = L"MyForm";
			this->Text = L"MyForm";
			this->Load += gcnew System::EventHandler(this, &MyForm::MyForm_Load);
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->pictureBox1))->EndInit();
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->dataGridView1))->EndInit();
			(cli::safe_cast<System::ComponentModel::ISupportInitialize^  >(this->dataGridView2))->EndInit();
			this->ResumeLayout(false);
			this->PerformLayout();

		}
#pragma endregion
private: System::Void MyForm_Load(System::Object^ sender, System::EventArgs^ e) {
    // Налаштування dataGridView1
    dataGridView1->Columns->Clear();
    dataGridView1->Columns->Add("ColOrig", "Початковий масив");

    // Налаштування dataGridView2 (тільки ОДИН стовпчик)
    dataGridView2->Columns->Clear();
    dataGridView2->Columns->Add("ColRes", "Результат"); 
    dataGridView2->Width = 150; // Можна зменшити ширину, бо стовпчик один
}
	private: System::Void button1_Click(System::Object^  sender, System::EventArgs^  e) {
				 // Очистити DataGridView
		 dataGridView1->Rows->Clear();

    // Додати n=10 рядків до DataGridView
		 dataGridView1->Rows->Add(n);

    // Заповнення масиву випадковими числами
		 Random^ rand = gcnew Random();
			for (int i = 0; i < n; i++) {
				 mas[i] = rand->Next(-100, 100);
				 dataGridView1->Rows[i]->Cells[0]->Value = mas[i]; // запис у рядки першого стовпця
				 dataGridView1->Rows[i]->Cells[0]->Style->BackColor = Color::Plum;
    }
			 }
private: System::Void button3_Click(System::Object^ sender, System::EventArgs^ e) {
    int max = mas[0]; // Припускаємо, що перший елемент — найбільший

    for (int i = 1; i < n; i++) {
        if (mas[i] > max) {
            max = mas[i]; // Оновлюємо максимум, якщо знайшли більше число
        }
    }

    // Вивід результату в label1
    label1->Text = "Найбільший елемент: " + max.ToString();
}
private: System::Void button2_Click(System::Object^ sender, System::EventArgs^ e) {
    // Очищуємо тільки рядки, колонку не чіпаємо (вона вже створена в Load)
    dataGridView2->Rows->Clear();
    dataGridView2->Rows->Add(n);

    // Копіюємо дані у тимчасовий масив
    int tempMas[100];
    for (int i = 0; i < n; i++) {
        tempMas[i] = mas[i];
    }

    // Сортування методом обміну (бульбашка)
    for (int i = 0; i < n - 1; i++) {
        for (int j = 0; j < n - i - 1; j++) {
            if (tempMas[j] > tempMas[j + 1]) {
                int temp = tempMas[j];
                tempMas[j] = tempMas[j + 1];
                tempMas[j + 1] = temp;
            }
        }
    }

    // Вивід у єдиний стовпець (Cells[0])
    for (int i = 0; i < n; i++) {
        dataGridView2->Rows[i]->Cells[0]->Value = tempMas[i];
        dataGridView2->Rows[i]->Cells[0]->Style->BackColor = Color::LightGreen;
    }
}

};
}
