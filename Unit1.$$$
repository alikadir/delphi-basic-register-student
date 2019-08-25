unit Unit1;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, ComCtrls, StdCtrls, ExtCtrls;

type
  TForm1 = class(TForm)
    cbobolum: TComboBox;
    btnekle: TButton;
    btnsil: TButton;
    btncik: TButton;
    Label1: TLabel;
    Label2: TLabel;
    Label3: TLabel;
    edadsoyad: TEdit;
    dtpkayittarihi: TDateTimePicker;
    lvwogrencilistesi: TListView;
    Image1: TImage;
    procedure FormCreate(Sender: TObject);
    procedure btnekleClick(Sender: TObject);
    procedure btnsilClick(Sender: TObject);
    procedure btncikClick(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}
{$J+}

procedure TForm1.FormCreate(Sender: TObject);
begin
cbobolum.ItemIndex:=0;
lvwogrencilistesi.ViewStyle:=vsreport;
lvwogrencilistesi.Columns.add;
lvwogrencilistesi.columns.items[0].caption:='Ad Soyad';
lvwogrencilistesi.Columns.Items[0].Width:=150;
lvwogrencilistesi.Columns.add;
lvwogrencilistesi.columns.items[1].caption:='Bölüm';
lvwogrencilistesi.Columns.Items[1].Width:=140;
lvwogrencilistesi.Columns.add;
lvwogrencilistesi.columns.items[2].caption:='Kayýt Tarihi';
lvwogrencilistesi.Columns.Items[2].Width:=90;
end;
procedure TForm1.btnekleClick(Sender: TObject);
const s:integer=0;
begin
 if lvwogrencilistesi.Items.Count=0 then s:=0;
 lvwogrencilistesi.items.add;
 lvwogrencilistesi.items.item[s].caption:=edadsoyad.text;
 lvwogrencilistesi.items.item[s].subitems.add(cbobolum.text);
 lvwogrencilistesi.items.item[s].subitems.add(datetostr(dtpkayittarihi.date));
 s:=s+1;
end;

procedure TForm1.btnsilClick(Sender: TObject);
begin
if lvwogrencilistesi.itemindex<0 then
showmessage('önce listeden birini seçin sonra sil deyin kardeþimmm..  oooo böyle olacaksa baþtan kapat programý çek git !! >:(')
else
lvwogrencilistesi.Items.Delete(lvwogrencilistesi.ItemIndex);
end;

procedure TForm1.btncikClick(Sender: TObject);
begin
showmessage ('yaptýðým deneme programýný kullandýðýnýz için çok thank you :))  ..  By alikadir®' );

close;
end;

end.
