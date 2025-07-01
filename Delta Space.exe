#include <iostream>
#include <windows.h>
#include <list>
#include <string>
#include <map>
#include <algorithm>
#include <typeinfo>
#include <cmath>

using namespace std;

int main()
{
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);

    bool c = true;
    list<string> consoleds;
    string code;
    string word;
    int numb = 1;
    bool workspace = false;
    bool method = false;
    map<string, string> varstr;
    map<string, int> varint;
    map<string, list<string>> arrstr;
    string typeoff;
    string namevar;
    string valuevar;
    int valueint;
    string vartowrite;
    string vartochange;
    string changedvalue;
    int changedintvalue;
    string vartypetowrite;
    string vartypetochange;
    string varmethod;
    string whichmethod;
    string findstring;
    string removestring;
    string changedvaluemethod;
    string input;
    string input2;
    int numberread = 0;
    list<string> made;
    list<string> madearr;
    int whereinputs[]= {};
    int sizearr = sizeof(whereinputs) / sizeof(*whereinputs);
    int action;
    int actiontwo;
    string actionvar;
    string append;
    int element;




    cout << "Delta Space 0.5/2025" << endl;
    while (c)
    {
        cout << numb << "  ";
        getline(cin, code);
        if (code == "type word:")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, word);
                consoleds.push_back(word);
                numb++;
            }
            else
            {
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }

        }
        else if (code == "release")
        {
            cout << endl;
            for (string n : consoleds)
            {
                cout << n << " ";
            }
            cout << endl;
            cout << "Session end";
            c = false;
        }
        else if (code == "attach Workspace")
        {
            workspace = true;
            numb ++;
        }
        else if (code == "attach Method")
        {
            method = true;
            numb++;
        }
        else if (code == "make var(")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, typeoff);
                numb++;
                if (typeoff == "string")
                {
                    cout << numb << "      ";
                    getline(cin, namevar);
                    if (find(made.begin(), made.end(), namevar) != made.end())
                    {
                        cout << endl;
                        cout << "Error V2: Varible with that name is already exist" << endl;
                        cout << endl;
                        numb++;
                    }
                    else
                    {
                        numb++;
                        cout << numb << "      ";
                        getline(cin, valuevar);
                        varstr[namevar] = valuevar;
                        numb ++;
                        cout << numb << "  )" << endl;
                        made.push_back(namevar);
                        numb ++;
                    }

                }
                else if (typeoff == "integer")
                {
                    cout << numb << "      ";
                    getline(cin, namevar);
                    if (find(made.begin(), made.end(), namevar) != made.end())
                    {
                        cout << endl;
                        cout << "Error V2: Varible with that name is already exist" << endl;
                        cout << endl;
                        numb++;
                    }
                    else
                    {
                        numb++;
                        cout << numb << "      ";
                        cin >> valueint;
                        varint[namevar] = valueint;
                        numb ++;
                        cout << numb << "  )" << endl;
                        made.push_back(namevar);
                        numb ++;
                        cin.ignore();
                    }

                }
                else
                {
                    numb ++;
                    cout << numb << "  )";
                    cout << endl;
                    cout << "Error V1: Type of data named " << typeoff << " doesn't exist" << endl;
                    cout << endl;
                    numb ++;
                }
            }
            else
            {
                numb++;
                cout << numb << "   )";
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;

            }
        }
        else if (code == "type var:")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetowrite);
                if (vartypetowrite == "string")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartowrite);
                    if (find(made.begin(), made.end(), vartowrite) != made.end())
                    {
                        consoleds.push_back(varstr[vartowrite]);
                        numb++;

                    }
                    else
                    {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else if (vartypetowrite == "integer")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartowrite);
                    if (find(made.begin(), made.end(), vartowrite) != made.end())
                    {
                        consoleds.push_back(to_string(varint[vartowrite]));
                        numb++;
                        cin.ignore();
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else
                {
                    numb ++;
                    cout << numb << "  )";
                    cout << endl;
                    cout << "Error V1: Type of data named " << typeoff << " doesn't exist" << endl;
                    cout << endl;
                    numb ++;
                }


            }
            else
            {
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }

        }
        else if (code == "change var:")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetochange);
                if (vartypetochange == "string")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartochange);
                     if (find(made.begin(), made.end(), vartochange) != made.end())
                     {
                        numb++;
                        cout << numb << "      ";
                        getline(cin, changedvalue);
                        varstr[vartochange] = changedvalue;
                        numb++;

                     }
                     else
                     {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                     }
                }
                else if (vartypetochange == "integer")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartochange);
                      if (find(made.begin(), made.end(), vartochange) != made.end())
                      {
                        numb++;
                        cout << numb << "      ";
                        cin >> changedintvalue;
                        varint[vartochange] = changedintvalue;
                        numb++;
                        cin.ignore();

                      }
                      else
                      {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                      }
                }

            }
        }
        else if (code == "type sentence:")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, word);
                consoleds.push_back(word);
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetowrite);
                if (vartypetowrite == "string")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartowrite);
                    if (find(made.begin(), made.end(), vartowrite) != made.end())
                    {
                        consoleds.push_back(varstr[vartowrite]);
                        numb++;
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else if (vartypetowrite == "integer")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartowrite);
                    if (find(made.begin(), made.end(), vartowrite) != made.end())
                    {
                        consoleds.push_back(to_string(varint[vartowrite]));
                        numb++;
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else
                {
                    numb ++;
                    cout << numb << "  )";
                    cout << endl;
                    cout << "Error V1: Type of data named " << typeoff << " doesn't exist" << endl;
                    cout << endl;
                    numb ++;
                }

            }
            else
            {
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
        }
        else if (code == "move next")
        {
            if (workspace == true)
            {
                consoleds.push_back("\n");
                numb++;
            }
            else
            {
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
        }
        else if (code == "move far")
        {
            if (workspace == true)
            {
                consoleds.push_back("\t");
                numb++;
            }
            else
            {
                cout << endl;
                cout << "Error L1: Lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
        }
        else if (code == "change log")
        {
            cout << endl;
            cout << "Delta Space 0.0: type, word, release" << endl;
            cout << "Delta Space 0.1: make, var, lib Workspace, type of data 'string'" << endl;
            cout << "Delta Space 0.2: change, type of data 'integer'" << endl;
            cout << "Delta Space 0.3: sentence, move, next, far" << endl;
            cout << "Delta Space 0.4: method, lengthof, find, rfind, to" << endl;
            cout << "Delta Space 0.41: add, minus, multiply, divide, iseven, sqrt, degree, module, roundm, roundl, logarithm, logarithm 10, sinus, cosine, tangent " << endl;
            cout << "Delta Space 0.5: arr, all, append, appbegin" << endl;
            cout << endl;
            numb++;
        }
        else if (code == "change var to method:")
        {
            if (method == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetochange);
                if (vartypetochange == "string")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartochange);
                    if (find(made.begin(), made.end(), vartochange) != made.end())
                    {
                        numb++;
                        cout << numb << "      ";
                        getline(cin, changedvaluemethod);
                        if (changedvaluemethod == "lengthof")
                        {
                            varstr[vartochange] = to_string(varstr[vartochange].length());
                            numb++;
                        }
                        else if (changedvaluemethod == "find")
                        {
                            numb++;
                            cout << numb << "     ";
                            getline(cin, findstring);
                            if (varstr[varmethod].find(findstring))
                            {
                                varstr[vartochange] = "unfound";
                                numb++;
                            }
                            else
                            {
                                varstr[vartochange] = to_string(varstr[vartochange].find(findstring));
                                numb++;
                            }
                        }
                        else if (changedvaluemethod == "rfind")
                        {
                            numb++;
                            cout << numb << "     ";
                            getline(cin, findstring);
                            varstr[vartochange] = to_string(varstr[vartochange].rfind(findstring));
                            numb++;;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error M1: String method named " << changedvaluemethod << " doesn't exist" << endl;
                            cout << endl;
                            numb++;
                        }

                     }
                     else
                     {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                     }
                }
                else if (vartypetochange == "integer")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartochange);
                    if (find(made.begin(), made.end(), vartochange) != made.end())
                    {
                        numb++;
                        cout << numb << "      ";
                        getline(cin, changedvaluemethod);
                        if (changedvaluemethod == "add")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> action;
                            varint[vartochange] += action;
                            numb++;
                        }
                        else if (changedvaluemethod == "minus")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> action;
                            varint[vartochange] -= action;
                            numb++;
                        }
                        else if (changedvaluemethod == "multiply")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> action;
                            varint[vartochange] = varint[vartochange] * action;
                            numb++;
                        }
                        else if (changedvaluemethod == "divide")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> action;
                            if (action == 0)
                            {
                                cout << endl;
                                cout << "Error A1: Division by 0 was declared" << endl;
                                cout << endl;
                            }
                            else
                            {
                                 varint[vartochange] = varint[vartochange] / action;
                                 numb++;
                            }

                        }
                        else if (changedvaluemethod == "iseven")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> action;
                            varint[vartochange] = varint[vartochange] % 2;
                            numb++;
                        }
                        else if (changedvaluemethod == "add var")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> actionvar;
                            if (find(made.begin(), made.end(), actionvar) != made.end())
                            {
                                varint[vartochange] += varint[actionvar];
                                numb++;
                            }
                            else
                            {
                                cout << endl;
                                cout << "Error V3: Varible with that name doesn't exist" << endl;
                                cout << endl;
                            }

                        }
                        else if (changedvaluemethod == "minus var")
                        {
                             numb ++;
                            cout << numb << "       ";
                            cin >> actionvar;
                            if (find(made.begin(), made.end(), actionvar) != made.end())
                            {
                                varint[vartochange] -= varint[actionvar];
                                numb++;
                            }
                            else
                            {
                                cout << endl;
                                cout << "Error V3: Varible with that name doesn't exist" << endl;
                                cout << endl;
                            }
                        }
                        else if (changedvaluemethod == "multiply var")
                        {
                            numb ++;
                            cout << numb << "       ";
                            cin >> actionvar;
                            if (find(made.begin(), made.end(), actionvar) != made.end())
                            {
                                varint[vartochange] *= varint[actionvar];
                                numb++;
                            }
                            else
                            {
                                cout << endl;
                                cout << "Error V3: Varible with that name doesn't exist" << endl;
                                cout << endl;
                            }
                        }
                        else if (changedvaluemethod == "divide var")
                        {
                          numb ++;
                            cout << numb << "       ";
                            cin >> actionvar;
                            if (find(made.begin(), made.end(), actionvar) != made.end())
                            {
                                varint[vartochange] /= varint[actionvar];
                                numb++;
                            }
                            else
                            {
                                cout << endl;
                                cout << "Error V3: Varible with that name doesn't exist" << endl;
                                cout << endl;
                            }
                        }
                        else if (changedvaluemethod == "sqrt")
                        {
                            varint[vartochange] = sqrt(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "degree")
                        {
                           numb++;
                            cout << numb << "     ";
                            getline(cin, actionvar);
                            if (find(made.begin(), made.end(), actionvar) != made.end())
                            {
                                varint[vartochange] = pow(varint[vartochange], varint[actionvar]);
                                numb++;
                            }
                            else
                            {
                                cout << endl;
                                cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                                cout << endl;
                                numb++;
                            }
                        }
                        else if (changedvaluemethod == "module")
                        {
                            varint[vartochange] = abs(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "roundm")
                        {
                            varint[vartochange] = ceil(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "roundl")
                        {
                            varint[vartochange] = floor(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "logarithm")
                        {
                            varint[vartochange] = log(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "logarithm 10")
                        {
                            varint[vartochange] = log10(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "sinus")
                        {
                            varint[vartochange] = sin(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "cosine")
                        {
                            varint[vartochange] = cos(varint[vartochange]);
                            numb++;
                        }
                        else if (changedvaluemethod == "tangent")
                        {
                            varint[vartochange] = tan(varint[vartochange]);
                            numb++;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error M2: Integer method named " << changedvaluemethod << " doesn't exist" << endl;
                            cout << endl;
                            numb++;
                        }

                     }
                     else
                     {
                        cout << endl;
                        cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                     }
                }
            else
            {
                numb ++;
                cout << numb << "  )";
                cout << endl;
                cout << "Error V1: Type of data named " << vartypetochange << " doesn't exist" << endl;
                cout << endl;
                numb ++;
            }

            }
            else if (method == false && workspace == false)
            {
                cout << endl;
                cout << "Error L2: libs METHOD and WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
            else if (method == false)
            {
                cout << endl;
                cout << "Error L3: lib METHOD haven't attached yet" << endl;
                cout << endl;
            }
            else if (workspace == false)
            {
                cout << endl;
                cout << "Error L1: lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
        }
        else if (code == "type string method:")
        {
            if (method == true)
            {
                numb++;
                cout << numb << "     ";
                getline(cin, varmethod);
                if (find(made.begin(), made.end(), varmethod) != made.end())
                {
                    numb++;
                    cout << numb << "     ";
                    getline(cin, whichmethod);
                    if (whichmethod == "lengthof")
                    {
                        consoleds.push_back(to_string(varstr[varmethod].length()));
                        numb++;
                    }
                    else if (whichmethod == "find")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, findstring);
                        if (varstr[varmethod].find(findstring))
                        {
                            consoleds.push_back("unfound");
                            numb++;
                        }
                        else
                        {
                            consoleds.push_back(to_string(varstr[varmethod].find(findstring)));
                            numb++;
                        }
                    }
                    else if (whichmethod == "rfind")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, findstring);
                        consoleds.push_back(to_string(varstr[varmethod].rfind(findstring)));
                        numb++;
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error M1: STRING method named " << whichmethod << " doesn't exist" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else
                {
                     cout << endl;
                     cout << "Error V3: Varible named " << vartowrite << " unfound" << endl;
                     cout << endl;
                     numb++;
                }
            }
            else if (method == false && workspace == false)
            {
                cout << endl;
                cout << "Error L2: libs METHOD and WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
            else if (method == false)
            {
                cout << endl;
                cout << "Error L3: lib METHOD haven't attached yet" << endl;
                cout << endl;
            }
            else if (workspace == false)
            {
                cout << endl;
                cout << "Error L1^ lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
            }
        }
        else if (code == "type integer method:")
        {
           if (method == true)
            {
                numb++;
                cout << numb << "     ";
                getline(cin, varmethod);
                if (find(made.begin(), made.end(), varmethod) != made.end())
                {
                    numb++;
                    cout << numb << "     ";
                    getline(cin, whichmethod);
                    if (whichmethod == "add")
                    {
                        numb++;
                        cout << numb << "     ";
                        cin >> action;
                        consoleds.push_back(to_string(varint[varmethod] + action));
                        numb++;
                    }
                    else if (whichmethod == "minus")
                    {
                        numb++;
                        cout << numb << "     ";
                        cin >> action;
                        consoleds.push_back(to_string(varint[varmethod] - action));
                        numb++;
                    }
                    else if (whichmethod == "multiply")
                    {
                        numb++;
                        cout << numb << "     ";
                        cin >> action;
                        consoleds.push_back(to_string(varint[varmethod] * action));
                        numb++;
                    }
                    else if (whichmethod == "divide")
                    {
                        numb++;
                        cout << numb << "     ";
                        cin >> action;
                        if (action == 0)
                        {
                                cout << endl;
                                cout << "Error A1: Division by 0 was declared" << endl;
                                cout << endl;
                        }
                        else
                        {
                          consoleds.push_back(to_string(varint[varmethod] / action));
                          numb++;
                        }

                    }
                    else if (whichmethod == "iseven")
                    {
                        numb++;
                        cout << numb << "     ";
                        consoleds.push_back(to_string(varint[varmethod] % 2));
                        numb++;
                    }
                    else if (whichmethod == "add var")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, actionvar);
                        if (find(made.begin(), made.end(), actionvar) != made.end())
                        {
                            consoleds.push_back(to_string(varint[varmethod] + varint[actionvar]));
                            numb++;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                            cout << endl;
                            numb++;
                        }

                    }
                    else if (whichmethod == "minus var")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, actionvar);
                        if (find(made.begin(), made.end(), actionvar) != made.end())
                        {
                            consoleds.push_back(to_string(varint[varmethod] - varint[actionvar]));
                            numb++;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                            cout << endl;
                            numb++;
                        }

                    }
                    else if (whichmethod == "multiply var")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, actionvar);
                        if (find(made.begin(), made.end(), actionvar) != made.end())
                        {
                            consoleds.push_back(to_string(varint[varmethod] * varint[actionvar]));
                            numb++;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                            cout << endl;
                            numb++;
                        }

                    }
                    else if (whichmethod == "divide var")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, actionvar);
                        if (find(made.begin(), made.end(), actionvar) != made.end())
                        {
                            if (varint[actionvar] == 0)
                            {
                                cout << endl;
                                cout << "Error A1: Division by 0 was declared" << endl;
                                cout << endl;
                            }
                            else
                            {
                               consoleds.push_back(to_string(varint[varmethod] / varint[actionvar]));
                               numb++;
                            }

                        }
                        else
                        {
                            cout << endl;
                            cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                            cout << endl;
                            numb++;
                        }

                    }
                    else if (whichmethod == "sqrt")
                    {
                        consoleds.push_back(to_string(sqrt(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "degree")
                    {
                        numb++;
                        cout << numb << "     ";
                        getline(cin, actionvar);
                        if (find(made.begin(), made.end(), actionvar) != made.end())
                        {
                            consoleds.push_back(to_string(pow(varint[varmethod], varint[actionvar])));
                            numb++;
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error V3: Varible named " << actionvar << " unfound" << endl;
                            cout << endl;
                            numb++;
                        }
                    }
                    else if (whichmethod == "module")
                    {
                        consoleds.push_back(to_string(abs(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "roundm")
                    {
                        consoleds.push_back(to_string(ceil(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "roundl")
                    {
                        consoleds.push_back(to_string(floor(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "logarithm")
                    {
                        consoleds.push_back(to_string(log(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "logarithm 10")
                    {
                        consoleds.push_back(to_string(log10(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "sinus")
                    {
                        consoleds.push_back(to_string(sin(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "cosine")
                    {
                        consoleds.push_back(to_string(cos(varint[varmethod])));
                        numb++;
                    }
                    else if (whichmethod == "tangent")
                    {
                        consoleds.push_back(to_string(tan(varint[varmethod])));
                        numb++;
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error M2: INTEGER method named " << whichmethod << " doesn't exist" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else
                {
                     cout << endl;
                     cout << "Error V3: Varible named " << varmethod << " unfound" << endl;
                     cout << endl;
                     numb++;
                }
            }
            else if (method == false && workspace == false)
            {
                cout << endl;
                cout << "Error L2: libs METHOD and WORKSPACE haven't attached yet" << endl;
                cout << endl;
                numb++;
            }
            else if (method == false)
            {
                cout << endl;
                cout << "Error L3: lib METHOD haven't attached yet" << endl;
                cout << endl;
            }
            else if (workspace == false)
            {
                cout << endl;
                cout << "Error L1^ lib WORKSPACE haven't attached yet" << endl;
                cout << endl;
            }
        }
        else if (code == "make arr(")
        {
             if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, typeoff);
                numb++;
                if (typeoff == "string")
                {
                    cout << numb << "      ";
                    getline(cin, namevar);
                    if (find(madearr.begin(), madearr.end(), namevar) != madearr.end())
                    {
                        cout << endl;
                        cout << "Error R1: Array with that name is already exist" << endl;
                        cout << endl;
                        numb++;
                    }
                    else
                    {
                        cout << numb << "  )" << endl;
                        madearr.push_back(namevar);
                        numb ++;
                    }

                }
            }
                else
                {
                    numb ++;
                    cout << numb << "  )";
                    cout << endl;
                    cout << "Error V1: Type of data named " << typeoff << " doesn't exist" << endl;
                    cout << endl;
                    numb ++;
                }
        }
        else if (code == "change arr:")
        {
            if (method)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetochange);
                if (vartypetochange == "string")
                {
                   numb++;
                    cout << numb << "      ";
                    getline(cin, vartochange);
                    if (find(madearr.begin(), madearr.end(), vartochange) != madearr.end())
                    {
                        numb++;
                        cout << numb << "      ";
                        getline(cin, changedvaluemethod);
                        if (changedvaluemethod == "append")
                        {
                            numb ++;
                            cout << numb << "      ";
                            getline(cin, append);
                            arrstr[vartochange].push_back(append);
                            numb ++;

                        }
                        else if (changedvaluemethod == "appbegin")
                        {
                            numb ++;
                            cout << numb << "      ";
                            getline(cin, append);
                            arrstr[vartochange].push_front(append);
                            numb ++;

                        }
                        }
                        else
                        {
                            cout << endl;
                            cout << "Error M3: Array method named " << changedvaluemethod << " doesn't exist" << endl;
                            cout << endl;
                            numb++;
                        }

                     }
                     else
                     {
                        cout << endl;
                        cout << "Error R2: Varible named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                     }
                }
            }
        else if (code == "type arr<all>:")
        {
            if (workspace == true)
            {
                numb++;
                cout << numb << "      ";
                getline(cin, vartypetowrite);
                if (vartypetowrite == "string")
                {
                    numb++;
                    cout << numb << "      ";
                    getline(cin, vartowrite);
                    if (find(madearr.begin(), madearr.end(), vartowrite) != madearr.end())
                    {
                        for (string n : arrstr[vartowrite])
                        {
                            consoleds.push_back(n);
                            numb++;
                        }
                    }
                    else
                    {
                        cout << endl;
                        cout << "Error R2: Array named " << vartowrite << " unfound" << endl;
                        cout << endl;
                        numb++;
                    }
                }
                else
                {
                    numb ++;
                    cout << numb << "  )";
                    cout << endl;
                    cout << "Error V1: Type of data named " << typeoff << " doesn't exist" << endl;
                    cout << endl;
                    numb ++;
                }

        }
        else
        {
            numb++;
        }
    }
        else
        {
            numb++;
        }
    }
    return 0;
}
