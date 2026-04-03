##  Specialer
## Descripción
Reception of Special has been cool to say the least. That's why we made an exclusive version of Special, called Secure Comprehensive Interface for Affecting Linux Empirically Rad, or just 'Specialer'. With Specialer, we really tried to remove the distractions from using a shell. Yes, we took out spell checker because of everybody's complaining. But we think you will be excited about our new, reduced feature set for keeping you focused on what needs it the most. Please start an instance to test your very own copy of Specialer.

Additional details will be available after launching your challenge instance.
## Solución
```
for file in *
do
  if [ -d "$file" ]; then
    echo "$file is a directory."
  elif [ -f "$file" ]; then
    echo "$file is a file."
  fi
done
```
```
for folder in abra ala sim
do
  cd "$folder"
  for file in *
  do
    if [ -d "$file" ]; then
      echo "$file: directory."
    elif [ -f "$file" ]; then
      echo "$folder/$file:"
      printf "%s " $(<$file) # input redirection; alternative to 'cat'
      printf "\n\n"
    fi
  done
  cd ..
done
```
el primer codigo es para tener cada directorio utilizable, y el ultimo es para encontrar en cual de los que se abrieron se encuentra la bandera 
picoCTF{y0u_d0n7_4ppr3c1473_wh47_w3r3_d01ng_h3r3_49193632}
## Notas
## Referencias