using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NewBehaviourScript : MonoBehaviour
{
     [SerializeField] KeyCode keyOne;
     [SerializeField] KeyCode keyTwo;
     [SerializeField] Vector3 moveDirection;

     private void Fixedupdate()
     {
         if (Input.GetKey(keyOne))
         {  
             GetComponent<Rigidbody>().velocity += moveDirection;
         }
         if (Input. GetKey(key Two))
         {
             GetComponent<Rigidbody>().velocity -= moveDirection;
         }
     }
 }
