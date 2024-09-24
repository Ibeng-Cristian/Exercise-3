# Exercise-3

"; // Read and display file contents using file_get_contents() $content = file_get_contents($grp5_tognorussell_ex3.php); echo "File Contents:
"; echo nl2br($content); // Display file contents with line breaks } else { echo "File '$grp5_tognorussell_ex3.php' does not exist.
"; // Create and write data to the file using file_put_contents() $data = "This is a sample content.\nThis is the second line."; file_put_contents($filename, $data); echo "File '$filename' created and data written.
"; } // Read file into an array using file() if (file_exists($grp5_tognorussell_ex3.php)) { $lines = file($grp5_tognorussell_ex3.php); echo "File Contents in Array Format:
"; foreach ($lines as $line_num => $line) { echo "Line $line_num: " . htmlspecialchars($line) . "
"; } } ?>
