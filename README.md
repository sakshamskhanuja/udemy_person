## Person

### Description

Write a class with the name <b>Person</b>. The class needs three fields (instance variables) with the names <b>firstName</b>, <b>lastName</b> of type <b>String</b> and <b>age</b> of type <b>int</b>.

Write the following methods (instance methods):

### Examples of input/output

<ul>
<li>Method named <b>getFirstName</b> without any parameters, it needs to return the value of the <b>firstName</b> field.</li>
<li>Method named <b>getLastName</b> without any parameters, it needs to return the value of the <b>lastName</b> field.</li>
<li>Method named <b>getAge</b> without any parameters, it needs to return the value of the <b>age</b> field.</li>
<li>Method named <b>setFirstName</b> with one parameter of type <b>String</b>, it needs to set the value of the <b>firstName</b> field.</li>
<li>Method named <b>setLastName</b> with one parameter of type <b>String</b>, it needs to set the value of the <b>lastName</b> field.</li>
<li>Method named <b>setAge</b> with one parameter of type <b>int</b>, it needs to set the value of the <b>age</b> field. If the parameter is less than 0 or greater than 100, it needs to set the <b>age</b> field value to 0.</li>
<li>Method named <b>isTeen</b> without any parameters, it needs to return <b>true</b> if the value of the <b>age</b> field is greater than 12 and less than 20, otherwise, return <b>false</b>.</li>
<li>Method named <b>getFullName</b> without any parameters, it needs to return the full name of the person.
<ul>
<li>In case both <b>firstName</b> and <b>lastName</b> fields are empty, Strings return an empty <b>String</b>.</li>
<li>In case <b>lastName</b> is an empty <b>String</b>, return <b>firstName</b>.</li>
<li>In case <b>firstName</b> is an empty <b>String</b>, return <b>lastName</b>.</li>
</ul>
</li>
</ul>

To check if a <b>String</b> is empty, use the method <b>isEmpty</b> from the <b>String</b> class. For example, <b>firstName.isEmpty()</b> returns <b>true</b> if the <b>String</b> is empty or in other words, when the <b>String</b> does not contain any characters.

### Test Code

    Person person = new Person();
    person.setFirstName("");   // firstName is set to empty string
    person.setLastName("");    // lastName is set to empty string
    person.setAge(10);
    System.out.println("fullName= " + person.getFullName());
    System.out.println("teen= " + person.isTeen());
    person.setFirstName("John");    // firstName is set to John
    person.setAge(18);
    System.out.println("fullName= " + person.getFullName());
    System.out.println("teen= " + person.isTeen());
    person.setLastName("Smith");    // lastName is set to Smith
    System.out.println("fullName= " + person.getFullName());

### Output

    fullName=
    teen= false
    fullName= John
    teen= true
    fullName= John Smith
