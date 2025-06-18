
LAB 1:IMPLEMENTATION OF GIT


 A.Installation of git


 B.configure Git initial
      ->git config --global user.name "Prasamsha Tripathi"
      ->git config --global user.email "prasamshatripathi@gmail.com"


C.Create a git repository
       i.local repository
          ->mkdir Agile
          ->cd Agile
          ->git init

        ii.Add lab files
           ->git add.
           ->git commit -m "initial commit :lab 1 files are added"

D.Make changes,commit changes,push to remote
         i.Make changes:Edit your files.

         ii.commit changes
               ->git add.
               ->git commit -m "added result section to agile"

         iii.Push to remote
                  ->git push




 #SAMPLE WORKFLOW OF GIT IMPLEMENTATION
    git init
    git add .
    git commit -m "initial commit for lab_1"
    git remote add origin https://github.com/prasamshatripathi/Agile.git