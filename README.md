using System;

public class simpledataklg
{
    static public void Main()
    {
      datakeluarga ok = new datakeluarga();
      datakeluarga ayahku = new Ayah();
      ayahku.Nama = "Fikri maliki assegaf bin malik";
      ayahku.Umur = gtw;
      ayahku.Nohp = +62kosong;
      Console.WriteLine("Data Ayah:");
      Console.WriteLine(ayahku.Nama);
      Console.WriteLine(ayahku.Umur);
      Console.WriteLine(ayahku.Nohp);
      ayahku.Hobi();
      datakeluarga ibuku = new Ibu();
      ibuku.Nama = "Dian";
      ibuku.Umur = 40;
      ibuku.Nohp = +6288235604361;
      Console.Write("Data Ibu:");
      Console.WriteLine(ibuku.Nama);
      Console.WriteLine(ibuku.Umur);
      Console.WriteLine(ibuku.Nohp);
      ibuku.Hobi();
      Console.WriteLine("Data Diriku");
      datakeluarga aku = new Anak();
      aku.Nama = "M syafiq afrizal";
      aku.Umur = 17;
      aku.Nohp = +6289514726498;
      Console.WriteLine(aku.Nama);
      Console.WriteLine(aku.Umur);
      Console.WriteLine(aku.Nohp);
      aku.Hobi();      
    }
    class datakeluarga 
    {
        private string nama;
        public string Nama
        {
            get { return nama;}
            set { nama = value;}
        }
        private int umur;
        public int Umur
        {
            get {return umur;}
            set {umur = value;}
        }
        private long nohp;
        public long Nohp
        {
            get {return nohp;}
            set {nohp = value;}
        }
        public virtual void Hobi()
        {
            Console.WriteLine("Hobi");
        }
    }
    class Ayah:datakeluarga
    {
        public override void Hobi()
        {
            Console.WriteLine("memancing");
        }
    }
    class Ibu:datakeluarga 
    {
        public override void Hobi()
        {
            Console.WriteLine("Bermain tik tok");
        }
    }
    class Anak:datakeluarga 
    {
        public override void Hobi()
        {
            Console.WriteLine("futsal");
        }
    }

}
