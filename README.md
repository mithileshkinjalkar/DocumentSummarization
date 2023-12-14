# DocumentSummarization
Document Summarization Using a Linear Algebra Approach and a SOTA Approach.

Course: DSC 210 - Numerical Linear Algebra

Instructor: Dr. Tsui-wei Weng

Instructions:

1. Ensure that the following libraries are installed in python 3 environment:

* nltk
* scikit-learn
* datasets
* rouge
* summarizer
* numpy
* pandas
* regex
* matplotlib

2. Open "DocumentSummarization-LSI.ipynb" and run all the cells.

**EDA Results**:
![image](https://github.com/mithileshkinjalkar/DocumentSummarization/assets/152033611/c9de6861-fb22-4a13-8184-4e10208fe6f9)

Average word count across all articles is 635.

**Results**:

**Linear Algebra Approach - LSI**

**Tokenization**

Before:

BOGOTA, Colombia (CNN) -- A key rebel commander and fugitive from a U.S. drug trafficking indictment was killed over the weekend in an air attack on a guerrilla encampment, the Colombian military said Monday. Alleged cocaine trafficker and FARC rebel Tomas Medina Caracas in an Interpol photo. Tomas Medina Caracas, known popularly as "El Negro Acacio," was a member of the high command of the Fuerzas Armadas Revolucionarias de Colombia and, according to Colombian and U.S. officials, helped manage the group\'s extensive cocaine trafficking network. He had been in the cross-hairs of the U.S. Justice Department since 2002. He was charged with conspiracy to import cocaine into the United States and manufacturing and distributing cocaine within Colombia to fund the FARC\'s 42-year insurgency against the government. U.S. officials alleged Medina Caracas managed the rebel group\'s sales of cocaine to international drug traffickers, who in turn smuggled it into the United States. He was also indicted in the United States along with two other FARC commanders in November 2002 on charges of conspiring to kidnap two U.S. oil workers from neighboring Venezuela in 1997 and holding one of them for nine months until a $1 million ransom was paid. Officials said the army\'s Rapid Response Force, backed by elements of the Colombian Air Force, tracked Medina Caracas down at a FARC camp in the jungle in the south of the country. "After a bombardment, the troops occupied the camp, and they\'ve found 14 dead rebels so far, along with rifles, pistols, communications equipment and ... four GPS systems," Defense Minister Juan Manuel Santos said at a news conference. "The death of \'El Negro Acacio\' was confirmed by various sources, including members of FARC itself." Medina Caracas commanded FARC\'s 16th Front in the southern departments of Vichada and Guainia. Established in 1964 as the military wing of the Colombian Communist Party, FARC is Colombia\'s oldest, largest, most capable and best-equipped Marxist rebel group, according to the U.S. Department of State. E-mail to a friend . Journalist Fernando Ramos contributed to this report.

After:
![image](https://github.com/mithileshkinjalkar/DocumentSummarization/assets/152033611/0dda58fe-d3c3-443c-9c66-0fa9bdeec7de)

![image](https://github.com/mithileshkinjalkar/DocumentSummarization/assets/152033611/993ca31b-c570-436f-84d5-53ae9ea31d7f)

**Generated Summary Indices**
![image](https://github.com/mithileshkinjalkar/DocumentSummarization/assets/152033611/7e90ed67-bb04-43dc-a214-f44be110e65d)

**Generated Summary**
![image](https://github.com/mithileshkinjalkar/DocumentSummarization/assets/152033611/4322da1f-1d62-4c6d-b306-117fcc3e2563)

Article:

BOGOTA, Colombia (CNN) -- A key rebel commander and fugitive from a U.S. drug trafficking indictment was killed over the weekend in an air attack on a guerrilla encampment, the Colombian military said Monday. Alleged cocaine trafficker and FARC rebel Tomas Medina Caracas in an Interpol photo. Tomas Medina Caracas, known popularly as "El Negro Acacio," was a member of the high command of the Fuerzas Armadas Revolucionarias de Colombia and, according to Colombian and U.S. officials, helped manage the group's extensive cocaine trafficking network. He had been in the cross-hairs of the U.S. Justice Department since 2002. He was charged with conspiracy to import cocaine into the United States and manufacturing and distributing cocaine within Colombia to fund the FARC's 42-year insurgency against the government. U.S. officials alleged Medina Caracas managed the rebel group's sales of cocaine to international drug traffickers, who in turn smuggled it into the United States. He was also indicted in the United States along with two other FARC commanders in November 2002 on charges of conspiring to kidnap two U.S. oil workers from neighboring Venezuela in 1997 and holding one of them for nine months until a $1 million ransom was paid. Officials said the army's Rapid Response Force, backed by elements of the Colombian Air Force, tracked Medina Caracas down at a FARC camp in the jungle in the south of the country. "After a bombardment, the troops occupied the camp, and they've found 14 dead rebels so far, along with rifles, pistols, communications equipment and ... four GPS systems," Defense Minister Juan Manuel Santos said at a news conference. "The death of 'El Negro Acacio' was confirmed by various sources, including members of FARC itself." Medina Caracas commanded FARC's 16th Front in the southern departments of Vichada and Guainia. Established in 1964 as the military wing of the Colombian Communist Party, FARC is Colombia's oldest, largest, most capable and best-equipped Marxist rebel group, according to the U.S. Department of State. E-mail to a friend . Journalist Fernando Ramos contributed to this report.

Summary:

four GPS systems," Defense Minister Juan Manuel Santos said at a news conference. "The death of 'El Negro Acacio' was confirmed by various sources, including members of FARC itself." Medina Caracas commanded FARC's 16th Front in the southern departments of Vichada and Guainia. He was also indicted in the United States along with two other FARC commanders in November 2002 on charges of conspiring to kidnap two U.S.

**Evaluation**:
[{'rouge-1': {'r': 0.3333333333333333, 'p': 0.1935483870967742, 'f': 0.24489795453561022}, 'rouge-2': {'r': 0.075, 'p': 0.043478260869565216, 'f': 0.05504586691355986}, 'rouge-l': {'r': 0.3333333333333333, 'p': 0.1935483870967742, 'f': 0.24489795453561022}}]

---

**BERTSUM**

**Generated Summary**

Article:

BOGOTA, Colombia (CNN) -- A key rebel commander and fugitive from a U.S. drug trafficking indictment was killed over the weekend in an air attack on a guerrilla encampment, the Colombian military said Monday. Alleged cocaine trafficker and FARC rebel Tomas Medina Caracas in an Interpol photo. Tomas Medina Caracas, known popularly as "El Negro Acacio," was a member of the high command of the Fuerzas Armadas Revolucionarias de Colombia and, according to Colombian and U.S. officials, helped manage the group's extensive cocaine trafficking network. He had been in the cross-hairs of the U.S. Justice Department since 2002. He was charged with conspiracy to import cocaine into the United States and manufacturing and distributing cocaine within Colombia to fund the FARC's 42-year insurgency against the government. U.S. officials alleged Medina Caracas managed the rebel group's sales of cocaine to international drug traffickers, who in turn smuggled it into the United States. He was also indicted in the United States along with two other FARC commanders in November 2002 on charges of conspiring to kidnap two U.S. oil workers from neighboring Venezuela in 1997 and holding one of them for nine months until a $1 million ransom was paid. Officials said the army's Rapid Response Force, backed by elements of the Colombian Air Force, tracked Medina Caracas down at a FARC camp in the jungle in the south of the country. "After a bombardment, the troops occupied the camp, and they've found 14 dead rebels so far, along with rifles, pistols, communications equipment and ... four GPS systems," Defense Minister Juan Manuel Santos said at a news conference. "The death of 'El Negro Acacio' was confirmed by various sources, including members of FARC itself." Medina Caracas commanded FARC's 16th Front in the southern departments of Vichada and Guainia. Established in 1964 as the military wing of the Colombian Communist Party, FARC is Colombia's oldest, largest, most capable and best-equipped Marxist rebel group, according to the U.S. Department of State. E-mail to a friend . Journalist Fernando Ramos contributed to this report.

Summary:

BOGOTA, Colombia (CNN) -- A key rebel commander and fugitive from a U.S. drug trafficking indictment was killed over the weekend in an air attack on a guerrilla encampment, the Colombian military said Monday. Alleged cocaine trafficker and FARC rebel Tomas Medina Caracas in an Interpol photo. Officials said the army's Rapid Response Force, backed by elements of the Colombian Air Force, tracked Medina Caracas down at a FARC camp in the jungle in the south of the country.

**Evaluation**:

[{'rouge-1': {'r': 0.5555555555555556, 'p': 0.3333333333333333, 'f': 0.4166666619791667}, 'rouge-2': {'r': 0.35, 'p': 0.18666666666666668, 'f': 0.24347825633270326}, 'rouge-l': {'r': 0.5555555555555556, 'p': 0.3333333333333333, 'f': 0.4166666619791667}}]
