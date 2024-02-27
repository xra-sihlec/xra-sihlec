using System;

class BusinessProfile
{
    public string BusinessName { get; set; }
    public string Address { get; set; }
    public string ContactNumber { get; set; }
    public string Email { get; set; }
    public string Website { get; set; }

    // Constructor to initialize the profile
    public BusinessProfile(string businessName, string address, string contactNumber, string email, string website)
    {
        BusinessName = businessName;
        Address = address;
        ContactNumber = contactNumber;
        Email = email;
        Website = website;
    }

    // Method to display the business profile information
    public void DisplayProfile()
    {
        Console.WriteLine($"Business Name: {BusinessName}");
        Console.WriteLine($"Address: {Address}");
        Console.WriteLine($"Contact Number: {ContactNumber}");
        Console.WriteLine($"Email: {Email}");
        Console.WriteLine($"Website: {Website}");
    }
}

class Program
{
    static void Main()
    {
        // Example usage
        BusinessProfile myBusiness = new BusinessProfile("ABC Corporation", "123 Main St", "555-1234", "info@abccorp.com", "www.abccorp.com");
        myBusiness.DisplayProfile();
    }
}
