# LinkedInCypressTesting
Test login with usser/password wrong

describe('LinkedIn',() =>{

it('Check if I get an error messaje',() => {

    cy.visit('https://linkedin.com');
    cy.get('.nav__button-secondary').click();
    cy.get('#username').type('ionrafaelstamatie@gmail.com');
    cy.get('#password').type('123456');                      // Nu am folosit parola corecta
    cy.get('.btn__primary--large').click(); 


    cy.get('#ember17').should('exsist');

})

})
