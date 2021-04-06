Welcome.

This is a maintained technical guide that aims to provide introduction to various online tracking techniques, online id verification techniques and guidance to creating and maintaining (truly) anonymous online identities including social media accounts safely and legally. No pre-requisites besides English reading are required.

This guide is an open-source non-profit initiative, [licensed] <sup>[[Mirror]][8]</sup> <sup>[[Archive.org]][9]</sup> under Creative Commons Attribution 4.0 International ([cc-by-4.0]) and is not sponsored/endorsed by any commercial/governmental entity.

The latest version is **0.8.9**, See the CHANGELOG at <https://anonymousplanet.org/CHANGELOG.html> <sup>[[Mirror]][10]</sup> <sup>[[Tor Mirror]][18]</sup>

Latest Online HTML versions at:
- Main: <https://anonymousplanet.org/guide.html> <sup>[[Archive.org]][6]</sup> <sup>[[Archive.today]][7]</sup> 
- Mirror: <https://mirror.anonymousplanet.org/guide.html> <sup>[[Archive.org]][5]</sup> <sup>[[Archive.today]][24]</sup> 
- Tor Mirror: <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion> 
- Archive.today over Tor: <http://archivecaslytosk.onion/anonymousplanet.org/guide.html>

Latests PDF versions at:
- (Light) <https://anonymousplanet.org/guide.pdf> <sup>[[Mirror]][1]</sup> <sup>[[Archive.org]][2]</sup> 
- (Light Tor Version) <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/guide.pdf> 
- (Dark) <https://anonymousplanet.org/guide-dark.pdf> <sup>[[Mirror]][3]</sup> <sup>[[Archive.org]][4]</sup> 
- (Dark Tor Version) <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/guide-dark.pdf>
- All latest PDFs are also available on CryptPad at <https://cryptpad.fr/drive/#/2/drive/view/Ughm9CjQJCwB8BIppdtvj5zy4PyE-8Gxn11x9zaqJLI/>

The PDF files in this guide have been checked by VirusTotal and Hybrid-Analysis, see the links below (**Note that this guide does not endorse VirusTotal/Hybrid-Analysis at all and it should be used with extreme caution and never with any sensitive files due to their privacy policy.**)
- (Light): [[VirusTotal]][light_virustotal], [[Hybrid-Analysis]][light_hybrid_analysis]
- (Dark): [[VirusTotal]][dark_virustotal], [[Hybrid-Analysis]][dark_hybrid_analysis]

In addition, you can always double check them using PDFID which you can download at <https://blog.didierstevens.com/programs/pdf-tools/>

- Install latest 3.9.x version of Python, Download PDFID and run:

```python pdfid.py file-to-check.pdf```

And you should see the following at 0:

```
/JS                    0 #This indicates the presence of Javascript
/JavaScript            0 #This indicates the presence of Javascript
/AA                    0 #This indicates the presence of automatic action on opening
/OpenAction            0 #This indicates the presence of automatic action on opening
/AcroForm              0 #This indicates the presence of AcroForm which could contain JavaScript
/JBIG2Decode           0 #This indicates the PDF uses JBIG2 compression which could be used for obfuscating malicious content
/RichMedia             0 #This indicates the presence rich media within the PDF such as Flash
/Launch                0 #This counts the launch actions
/EmbeddedFile          0 #This indicates there are embedded files within the PDF
/XFA                   0 #This indicates the presence of XML Forms within the PDF
```

SHA256 Checksums of all the PDFs are available here: 
- Main and Mirror: <https://anonymousplanet.org/sha256sum.txt> <sup>[[Mirror]][11]</sup>
- Tor Mirror: <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/sha256sum.txt>

SHA256 Checksums and GPG keys of the full repository releases files are available within the checksum file at <https://github.com/AnonymousPlanet/thgtoa/releases/latest>

The GPG signatures for each PDF file are available here:
- (Light) Main and Mirror: <https://anonymousplanet.org/guide.pdf.asc> <sup>[[Mirror]][20]</sup>
- (Light) Tor Mirror: <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/guide.pdf.asc>
- (Dark) Main and Mirror: <https://anonymousplanet.org/guide-dark.pdf.asc>  <sup>[[Mirror]][21]</sup>
- (Dark) Tor Mirror: <http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/guide-dark.pdf.asc>

To check the SHA256 Checksums please do the following:

Windows:
- From a command prompt, run ```certutil -hashfile filename.txt sha256```
- Compare the result with the hash in the checksum files.

MacOS:
- From a terminal, run ```shasum -a 256 /full/path/to/your/file```
- Compare the result with the hash in the checksum files.

Linux: 
- From a terminal, ```run sha256sum /full/path/to/your/file```
- Compare the result with the hash in the checksum files.

All commits and releases on this repository are signed and verified using the same key. Check for the "Verified" tags.

If you don't know how to verify files with GGP signatures, you should first install gpg on your system:
- Windows: Install gpg4win from <https://www.gpg4win.org/download.html>
- MacOS: Install GPG Tools from <https://gpgtools.org/>
- Linux: gpg should be installed by default

Import the GPG key using the following command from a command prompt or terminal:

```gpg --auto-key-locate nodefault,wkd --locate-keys 0xEB16B6AB4AB7BA61F33E2DFD0051E9A589DAB601```

If this doesn't work, you can also download/view it directly from here: <https://anonymousplanet.org/AnonymousPlanet_0x89DAB601_public.asc> <sup>[[Mirror]][12]</sup> <sup>[[Tor Mirror]][17]</sup>

And then import it manually by issuing the following command:

```gpg --import AnonymousPlanet_0x89DAB601_public.asc```

Finally, verify the files by issuing the following commands: 

```gpg --verify guide.pdf.asc guide.pdf"```
```gpg --verify guide-dark.pdf.asc guide-dark.pdf"```

You can also verify the authenticity of this GPG signature using:
- My Keybase.io profile <https://keybase.io/anonymousplanet>
- My Keyoxide.org profile <https://keyoxide.org/eb16b6ab4ab7ba61f33e2dfd0051e9a589dab601>

As well as the published key on (Search for the Fingerprint):
- <http://keys.gnupg.net>
- <https://pgp.mit.edu>
- <https://keys.openpgp.org>
- <https://keyserver.ubuntu.com> 

Using the following GPG fingerprint: ```0xEB16B6AB4AB7BA61F33E2DFD0051E9A589DAB601```

Feel free to submit issues using Github Issues or discuss using Github Discussions.

If you'd like to make a donation to this project, you can do so from <https://anonymousplanet.org/donations.html> <sup>[[Mirror]][13]</sup> <sup>[[Tor Mirror]][19]</sup>

Follow or contact me on: 
- Twitter: <https://twitter.com/AnonyPla> (cannot guarantee this account will stay up for long tho)
- Mastodon: <https://mastodon.online/@anonypla>
- Element/Matrix.org: ```@anonypla:privacytools.io```
- Reddit: <https://old.reddit.com/message/compose/?to=AnonyPla>
- E-Mail: <contact@anonymousplanet.org>

Discussion Channels (**be careful as none of those are actively moderated**):
- Reddit: <https://old.reddit.com/r/thgtoa/>
- Discord Server: <https://discord.gg/XGFfGtJmXd>
- Github Discussions: <https://github.com/AnonymousPlanet/thgtoa/discussions>

Have a good read and feel free to share it!

[cc-by-4.0]: https://creativecommons.org/licenses/by/4.0/
[licensed]: https://anonymousplanet.org/LICENSE.html
[light_virustotal]: https://www.virustotal.com/gui/file/037313de01fe22f6fd6244cd55759741c6d6adaecd174a9b8c282060d2c0bbf3/detection
[light_hybrid_analysis]: https://hybrid-analysis.com/sample/037313de01fe22f6fd6244cd55759741c6d6adaecd174a9b8c282060d2c0bbf3
[dark_virustotal]: https://www.virustotal.com/gui/file/5dbeca50403e83c846f5d1d25d9705b3b2ba9bd38b1e1a1bdae155a038e7a550/detection
[dark_hybrid_analysis]: https://hybrid-analysis.com/sample/5dbeca50403e83c846f5d1d25d9705b3b2ba9bd38b1e1a1bdae155a038e7a550
[1]: https://mirror.anonymousplanet.org/guide.pdf 
[2]: https://web.archive.org/web/https://anonymousplanet.org/guide.pdf
[3]: https://mirror.anonymousplanet.org/guide-dark.pdf 
[4]: https://web.archive.org/web/https://anonymousplanet.org/guide-dark.pdf
[5]: https://web.archive.org/web/https://mirror.anonymousplanet.org/guide.html
[6]: https://web.archive.org/web/https://anonymousplanet.org/guide.html
[7]: https://archive.fo/anonymousplanet.org/guide.html
[8]: https://mirror.anonymousplanet.org/LICENSE.html
[9]: https://web.archive.org/web/https://anonymousplanet.org/LICENSE.html
[10]: https://mirror.anonymousplanet.org/CHANGELOG.html
[11]: https://mirror.anonymousplanet.org/sha256sum.txt
[12]: https://mirror.anonymousplanet.org/AnonymousPlanet_0x89DAB601_public.asc
[13]: https://mirror.anonymousplanet.org/donations.html



[17]: http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/AnonymousPlanet_0x89DAB601_public.asc
[18]: http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/CHANGELOG.html
[19]: http://thgtoa7imksbg7rit4grgijl2ef6kc7b56bp56pmtta4g354lydlzkqd.onion/donations.html
[20]: https://mirror.anonymousplanet.org/guide.pdf.asc
[21]: https://mirror.anonymousplanet.org/guide-dark.pdf.asc


[24]: https://archive.fo/mirror.anonymousplanet.org/guide.html