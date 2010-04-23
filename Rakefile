task :default do
  puts "Doing nothing"
end

desc "Compile Android version"
task :android do
  puts "Not implemented yet"
end

desc "Compile x86 version"
task :x86 do
  Tools.execute "make distclean"
  Tools.execute "./configure --prefix=/home/mark/Work/brewedcast/out/x86 --enable-optimize --enable-http --enable-ftp --enable-file --disable-ldap --disable-rtsp --enable-proxy --disable-dict --disable-telnet --disable-tftp --disable-pop3 --disable-imap --disable-smtp --disable-manual --disable-ipv6 --enable-nonblocking --disable-sspi --enable-cookies --with-ssl=/usr --with-zlib --without-nss"
  Tools.execute "make"
  Tools.execute "make install"
end

module Tools
  def self.execute(cmd)
    puts(cmd)
    system(cmd)
  end
end
