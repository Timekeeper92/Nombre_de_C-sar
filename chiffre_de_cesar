puts "Bienvenue au chiffre de César!"
puts "Enter 'quit' to exit the program"

def chiffre_de_cesar(user_string, shift_factor)
  user_string.length.times do |index| 
    if /[a-z]/.match(user_string[index])
      letter = user_string[index].ord + shift_factor
      if letter > "z".ord
        user_string[index] = (letter - 26).chr
      else
        user_string[index] = letter.chr
      end
    elsif /[A-Z]/.match(user_string[index])
      letter = user_string[index].ord + shift_factor
      if letter > "Z".ord
        user_string[index] = (letter - 26).chr
      else
        user_string[index] = letter.chr
      end
    end
  end
  return user_string
end

while true
  puts "Quelle methode voulez-vous cripter? "
  user_string = gets.chomp
  
  if user_string.downcase == 'quit'
    break
  else
    puts "Quel facteur voulez-vous utiliser? "
    shift_factor = gets.to_i
    user_string = caesar_cipher(user_string, shift_factor)
    
    puts user_string
  end
end