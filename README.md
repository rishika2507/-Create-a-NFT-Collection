// Create a variable to hold your NFTs
let NFTs = [];

// This function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT(name, eyecolor, shirtType, bling) {
    const NFT = {
        name: name,
        eyecolor: eyecolor,
        shirtType: shirtType,
        bling: bling
    };
    NFTs.push(NFT);
   }

// Create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs() {
    for (let i = 0; i < NFTs.length; i++) {
        console.log('NFT #'+(i+ 1));
        console.log('  Name: '+NFTs[i].name);
        console.log('  eyecolor: '+NFTs[i].eyecolor);
        console.log('  shirtType: '+NFTs[i].shirtType);
        console.log('  bling: '+NFTs[i].bling);
    }
}

// Print the total number of NFTs we have minted to the console
function getTotalSupply() {
    console.log('Total NFTs Minted:' +NFTs.length);
}


// Declare a few NFTs beforehand
mintNFT('Rishika', 'brown', 'linen', 'sparkle');
mintNFT('Reem', 'black', 'check', 'plain');
mintNFT('Rash', 'hazel', 'plaid', 'plain');
mintNFT('Risa', 'green', 'cotton', 'cheap');

// Calling the function with the details of NFTS
listNFTs();

// Calling the function to print the total number of NFTs 
getTotalSupply();




