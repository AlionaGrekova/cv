# Aliona Grekova
### Contact information:
Phone: +375298122559

E-mail: nikagrek15@gmail.com

Telegram: @Ali_o_nka

[VK](https://vk.com/all_enchik)

### About Myself:
Speaking of qualities, I consider myself responsible, smart, disciplined, intelligent. I graduated from school with a silver medal. Now I'm studying at the university on the specialty "Management of information resources". I managed to work in the interactive museum "Festival Robotov". There I told children and adults about various robots, how they work, what they can do.
### Skills and Proficiency:
- HTML
- C++
- Git, GitHub
- Adobe Photoshop, Inkscape, Blender
### Code example:
Task: find the sum of the elements of each diagonal of an N×N square array parallel to the side diagonal, and the minimum of the found values

void find_min_sum(int **mm, int *ss,int raz)
{
    

    int k, itog;
    for (k = 0; k < raz - 1; k++)
    {

        ss[k] = 0;
        for (int i = 0; i <= k; i++)
        {

            ss[k] = ss[k] + mm[i][k - i];
        }
    }

    for (k = raz; k <= (raz - 1) * 2; k++)
    {
        ss[k - 1] = 0;
        for (int i = (raz - 1); i >= k - raz + 1; i--)
        {
            ss[k - 1] = ss[k - 1] + mm[k - i][i];
        }

    }

    for (int i = 0; i < (raz - 1) * 2; i++)
    {
        if (i == 0) { itog = ss[0]; }
        else
        {
            if (itog > ss[i]) { itog = ss[i]; }

        }
        cout << "\nСумма " << i + 1 << " диагонали - " << ss[i];
    }

    cout << "\nМинимальное из сумм диагоналей, параллельных побочной диагонали - " << itog << "\n";
}
### Languages:
I studied English at school and continue to study at the university
