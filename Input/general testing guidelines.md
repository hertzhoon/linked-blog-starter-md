Be more specific with what you are asserting.
Assert as much as possible, while still within the scope of the use case.
Asserting two objects equal -> assertThat().usingRecursiveComparison()

Exceptions
	JUnit4 -> @Rule public ExpectedException thrown = ExpectedException.none();
	JUnit5 -> assertThrows()