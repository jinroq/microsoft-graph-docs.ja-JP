---
title: Microsoft Graph の People API を使用した最も関連のある人物に関する情報の取得
description: Graph のアプリケーションでは、ユーザーに最も関連する人を取得するためにユーザーの API を使用できます。 関連性は、ユーザーのコミュニケーションとコラボレーションのパターンとビジネスの関係によって決定されます。 ローカルの連絡先、取引先担当者からソーシャル ネットワークまたは組織のディレクトリから、およびユーザーの最新の通信 (電子メール、Skype など) ことがあります。 人 API と、この情報を生成するには、あいまい一致検索のサポートと、サインイン中のユーザーの組織内の別のユーザーに関連するユーザーの一覧を取得する機能も提供します。
ms.date: 12/04/2018
ms.openlocfilehash: b01ca4538c3155bbb30224b1f92d6e7ae55c5878
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156055"
---
# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a><span data-ttu-id="15e2e-106">Microsoft Graph の People API を使用した最も関連のある人物に関する情報の取得</span><span class="sxs-lookup"><span data-stu-id="15e2e-106">Use the People API in Microsoft Graph to get information about the people most relevant to you</span></span>

<span data-ttu-id="15e2e-p102">Microsoft Graph では、People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。この情報を生成するとともに、People API は、ファジー マッチ検索のサポートと、サインインしているユーザーの組織内の別のユーザーに関連するユーザーのリストを取得する機能も提供します。People API は、電子メールの作成や会議の作成などのシナリオを選択するユーザーに特に便利です。たとえば、電子メール作成のシナリオで People API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p102">Microsoft Graph applications can use the People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. People can be local contacts, contacts from social networking or from an organization’s directory, and people from recent communications (such as email and Skype). Along with generating this insight, the People API also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed-in user's organization. The People API is particularly useful for people picking scenarios, such as composing an email or creating a meeting. For example, you can use the People API in email compose scenarios.</span></span>

## <a name="authorization"></a><span data-ttu-id="15e2e-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="15e2e-113">Authorization</span></span>

<span data-ttu-id="15e2e-114">Microsoft Graph で People API を呼び出すには、アプリに適切なアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="15e2e-114">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="15e2e-p103">People.Read - 一般的な People API の呼び出し (例: `https://graph.microsoft.com/v1.0/me/people/`) の作成に使用します。People.Read には、エンド ユーザーの同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p103">People.Read - Use to make general People API calls; for example, `https://graph.microsoft.com/v1.0/me/people/`. People.Read requires end user consent.</span></span>
* <span data-ttu-id="15e2e-117">People.Read.All - ログインしているユーザーの組織内の指定されたユーザーに最も関連する人を取得するために必要な (`https://graph.microsoft.com/v1.0/users('{id}')/people`) の呼び出し。</span><span class="sxs-lookup"><span data-stu-id="15e2e-117">People.Read.All - Required to retrieve the people most relevant to a specified user in the signed-in user’s organization (`https://graph.microsoft.com/v1.0/users('{id}')/people`) calls.</span></span> <span data-ttu-id="15e2e-118">People.Read.All には、管理者の承認が必要です。</span><span class="sxs-lookup"><span data-stu-id="15e2e-118">People.Read.All requires admin consent.</span></span>

## <a name="browse-people"></a><span data-ttu-id="15e2e-119">人物の参照</span><span class="sxs-lookup"><span data-stu-id="15e2e-119">Browse people</span></span>

<span data-ttu-id="15e2e-p105">このセクションの要求では、サインインしているユーザー (`/me`)、またはサインインしているユーザーの組織内の特定のユーザーと最も関連性の高い人物を取得します。これらの要求には People.Read または People.Read.All アクセス許可が必要です。既定では、応答ごとに 10 件のレコードが返されますが、これは *$top* クエリ パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p105">The requests in this section get the people most relevant to the signed-in user (`/me`), or to a specific user in the signed-in user’s organization. These requests require the People.Read or People.Read.All permission respectively. By default, each response returns 10 records, but you can change this by using the *$top* query parameter.</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="15e2e-123">関連する人物のコレクションの取得</span><span class="sxs-lookup"><span data-stu-id="15e2e-123">Get a collection of relevant people</span></span>

<span data-ttu-id="15e2e-124">次に示す要求では、コミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップに基づいて、サインインしているユーザーに最も関連のある人物を取得します (`/me`)。</span><span class="sxs-lookup"><span data-stu-id="15e2e-124">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="15e2e-p106">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* クエリ パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p106">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "givenName": "Lorrie",
      "surname": "Frye",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Paralegal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "20/1109",
      "profession": "",
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 980 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "givenName": "Maynard",
      "surname": "Denman",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Web Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/1101",
      "profession": "",
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "givenName": "Darrel",
      "surname": "Halsey",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Attorney",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "14/1102",
      "profession": "",
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 205 555 0103"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="request-a-subsequent-page-of-people"></a><span data-ttu-id="15e2e-129">人物の続きのページの要求</span><span class="sxs-lookup"><span data-stu-id="15e2e-129">Request a subsequent page of people</span></span>

<span data-ttu-id="15e2e-p107">最初の応答に関連のある人物のリストを完全に含められない場合は、追加の情報ページを要求するために、*$top* と *$skip* を使用して 2 番目の要求を行うことができます。前の要求に追加情報が含まれている場合は、次の要求でサーバーから人物についての後続ページを取得します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p107">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

<span data-ttu-id="15e2e-p108">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* クエリ パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1F28616D-BDFE-4080-8F06-03366A851688",
      "displayName": "Felix Coppola",
      "givenName": "Felix",
      "surname": "Coppola",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "CVP Legal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "19/2109",
      "profession": "",
      "userPrincipalName": "FelixC@contoso.onmicrosoft.com",
      "imAddress": "sip:FelixC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "FelixC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 309 555 0104"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
      "displayName": "Lenora Rowland",
      "givenName": "Lenora",
      "surname": "Rowland",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Marketing Assistant",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "18/1106",
      "profession": "",
      "userPrincipalName": "LenoraR@contoso.onmicrosoft.com",
      "imAddress": "sip:LenoraR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LenoraR@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 954 555 0118"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
      "displayName": "Manuel Collette",
      "givenName": "Manuel",
      "surname": "Collette",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Accountant II",
      "companyName": null,
      "yomiCompany": "",
      "department": "Finance",
      "officeLocation": "98/2202",
      "profession": "",
      "userPrincipalName": "ManuelC@contoso.onmicrosoft.com",
      "imAddress": "sip:ManuelC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ManuelC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+20 255501070"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="sort-the-response"></a><span data-ttu-id="15e2e-136">応答の並べ替え</span><span class="sxs-lookup"><span data-stu-id="15e2e-136">Sort the response</span></span>

<span data-ttu-id="15e2e-p109">既定では、応答に含まれる人物は、クエリとの関連性で並べ替えられます。応答に含まれる人物の順序は、*$orderby* パラメーターを使用することで変更できます。このクエリでは、自分に最も関連のある人物を選択し、その人物を **displayName** で並べ替えてから、最初の 10 人の人物を並べ替え済みのリストで返します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p109">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their **displayName**, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

<span data-ttu-id="15e2e-p110">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。次の例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. The following example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
      "displayName": "Adriana Ramos",
      "givenName": "Adriana",
      "surname": "Ramos",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Product Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "18/2111",
      "profession": "",
      "userPrincipalName": "AdrianaR@contoso.onmicrosoft.com",
      "imAddress": "sip:AdrianaR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AdrianaR@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 425 555 0109"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
      "displayName": "Alyce Cooley",
      "givenName": "Alyce",
      "surname": "Cooley",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Marketing Assistant",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "131/1104",
      "profession": "",
      "userPrincipalName": "AlyceC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyceC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyceC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 858 555 0110"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
      "displayName": "Alyssa Clarke",
      "givenName": "Alyssa",
      "surname": "Clarke",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Corporate Security Officer",
      "companyName": null,
      "yomiCompany": "",
      "department": "Operations",
      "officeLocation": "24/1106",
      "profession": "",
      "userPrincipalName": "AlyssaC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyssaC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyssaC@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 262 555 0106"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="change-the-number-of-people-and-fields-returned"></a><span data-ttu-id="15e2e-144">返される人物の数とフィールド数の変更</span><span class="sxs-lookup"><span data-stu-id="15e2e-144">Change the number of people and fields returned</span></span>

<span data-ttu-id="15e2e-145">応答で返される人物の数は、*$top* パラメーターを設定することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-145">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="15e2e-p111">次に示す例では、`/me` に最も関連のある 1,000 人の人物を要求します。また、この要求では、人物の **displayName** のみを要求することで、サーバーから返されるデータの量も制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p111">The following example requests the 1,000 people most relevant to `/me`. The request also limits the amount of data sent back from the server by requesting only the **displayName** of the person.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

<span data-ttu-id="15e2e-148">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-148">The following example shows the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye"
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman"
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey"
    },
    {
      "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
      "displayName": "Roscoe Seidel"
    },
    {
      "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
      "displayName": "Alyssa Clarke"
    },
    {
      "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
      "displayName": "Adriana Ramos"
    },
    {
      "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
      "displayName": "Alyce Cooley"
    },
    {
      "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
      "displayName": "Wayne Leeper"
    },
    {
      "id": "E7D40AC5-0078-4575-B1F3-F738124C4BC9",
      "displayName": "Jan Travis"
    },
    {
      "id": "6F99D1CC-4FCC-49E4-9160-E8AB01BF3E83",
      "displayName": "Charlotte Delacruz"
    },
    {
      "id": "1F28616D-BDFE-4080-8F06-03366A851688",
      "displayName": "Felix Coppola"
    },
    {
      "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
      "displayName": "Lenora Rowland"
    },
    {
      "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
      "displayName": "Manuel Collette"
    }
  ]
}
```

### <a name="select-the-fields-to-return"></a><span data-ttu-id="15e2e-149">返されるフィールドの選択</span><span class="sxs-lookup"><span data-stu-id="15e2e-149">Select the fields to return</span></span>

<span data-ttu-id="15e2e-p112">サーバーから返されるデータの量は、1 つ以上のフィールドを選択する *$select* パラメーターを使用することで制限できます。`@odata.id` フィールドは常に返されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p112">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The `@odata.id` field is always returned.</span></span>

<span data-ttu-id="15e2e-152">次に示す例では、最も関連のある 10 人の人物の **displayName** と **scoredEmailAddresses** に応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-152">The following example limits the response to the **displayName** and **scoredEmailAddresses** of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

<span data-ttu-id="15e2e-p113">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p113">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="use-a-filter-to-limit-the-response"></a><span data-ttu-id="15e2e-157">フィルターを使用した応答の制限</span><span class="sxs-lookup"><span data-stu-id="15e2e-157">Use a filter to limit the response</span></span>

<span data-ttu-id="15e2e-158">*$filter* パラメーターを使用すると、指定した条件に等しいレコードを持つ人物のみに応答を制限できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-158">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="15e2e-159">次のクエリは、**class** として **person**、**subclass** として **organizationUser** が割り当てられている **personType** プロパティを持つ **person** インスタンスへの応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-159">The following query limits the response to **person** instances with the **personType** property being assigned **person** as **class** and **organizationUser** as **subclass**.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

<span data-ttu-id="15e2e-p114">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p114">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "givenName": "Lorrie",
      "surname": "Frye",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Paralegal",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "20/1109",
      "profession": "",
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 980 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "givenName": "Maynard",
      "surname": "Denman",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Web Marketing Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/1101",
      "profession": "",
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "givenName": "Darrel",
      "surname": "Halsey",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Attorney",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "14/1102",
      "profession": "",
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 205 555 0103"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="15e2e-164">フィルター処理された応答で返されるフィールドを選択する</span><span class="sxs-lookup"><span data-stu-id="15e2e-164">Select the fields to return in a filtered response</span></span>

<span data-ttu-id="15e2e-165">*$select* パラメーターと *$filter* パラメーターを組み合わせることで、ユーザーに関連のある人物のカスタム リストを作成し、アプリケーションで必要になるフィールドのみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-165">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="15e2e-p115">次の例では、指定した名前と等しい表示名を持つ人物の **displayName** と **scoredEmailAddresses** を取得します。この例では、表示名が "Lorrie Frye" と等しい人物のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p115">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="15e2e-168">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-168">The following example shows the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
      "displayName": "Lorrie Frye",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="browse-another-users-relevant-people"></a><span data-ttu-id="15e2e-169">他のユーザーの関連する人物の参照</span><span class="sxs-lookup"><span data-stu-id="15e2e-169">Browse another user’s relevant people</span></span>

<span data-ttu-id="15e2e-170">次の要求は、サインインしているユーザーの組織内の他の人物と最も関連のある人物を取得します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-170">The following request gets the people most relevant to another person in the signed-in user's organization.</span></span> <span data-ttu-id="15e2e-171">この要求には People.Read.All アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="15e2e-171">This request requires the People.Read.All permission.</span></span> <span data-ttu-id="15e2e-172">上記のセクションで説明されているすべてのクエリ パラメーターに適用されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-172">All the query parameters described in the above sections apply as well.</span></span>

<span data-ttu-id="15e2e-173">この例では、Roscoe Seidel の関連する人物が表示されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-173">In this example, Roscoe Seidel's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="15e2e-p117">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。次に示す例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p117">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. The example below uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "56155636-703F-47F2-B657-C83F01F49BBC",
      "displayName": "Clifton Clemente",
      "givenName": "Clifton",
      "surname": "Clemente",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Director",
      "companyName": null,
      "yomiCompany": "",
      "department": "Legal",
      "officeLocation": "19/2106",
      "profession": "",
      "userPrincipalName": "CliftonC@contoso.onmicrosoft.com",
      "imAddress": "sip:CliftonC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "CliftonC@contoso.onmicrosoft.com",
          "relevanceScore": 20
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 309 555 0101"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
      "displayName": "Sheree Mitchell",
      "givenName": "Sheree",
      "surname": "Mitchell",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "Product Manager",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "20/2107",
      "profession": "",
      "userPrincipalName": "ShereeM@contoso.onmicrosoft.com",
      "imAddress": "sip:ShereeM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ShereeM@contoso.onmicrosoft.com",
          "relevanceScore": 10
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 918 555 0107"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
      "displayName": "Vincent Matney",
      "givenName": "Vincent",
      "surname": "Matney",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "CVP Engineering",
      "companyName": null,
      "yomiCompany": "",
      "department": "Engineering",
      "officeLocation": "23/2102",
      "profession": "",
      "userPrincipalName": "VincentM@contoso.onmicrosoft.com",
      "imAddress": "sip:VincentM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "VincentM@contoso.onmicrosoft.com",
          "relevanceScore": 10
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 502 555 0102"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

## <a name="search-people"></a><span data-ttu-id="15e2e-178">人物の検索</span><span class="sxs-lookup"><span data-stu-id="15e2e-178">Search people</span></span>

<span data-ttu-id="15e2e-p118">このセクションの要求では、サインインしているユーザー (`/me`) とサインインしているユーザーの組織内の他のユーザーに関連する人物を検索できます。これらの要求には People.Read アクセス許可が必要です。ただし、他のユーザーに関連する人物を検索する場合は People.Read.All が必要です。既定では、応答ごとに 10 件のレコードが返されますが、これは *$top* パラメーターを使用することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p118">The requests in this section allow you to search for people relevant to the signed-in user (`/me`) and other users in the signed-in user’s organization. These requests require the People.Read permission, with the exception of searching other users’ relevant people, which requires People.Read.All. By default, each response returns 10 records, but you can change this by using the *$top* parameter.</span></span>

### <a name="use-search-to-select-people"></a><span data-ttu-id="15e2e-182">検索による人物の選択</span><span class="sxs-lookup"><span data-stu-id="15e2e-182">Use search to select people</span></span>

<span data-ttu-id="15e2e-183">*$search* パラメーターを使用して、特定の条件セットを満たす人物を選びます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-183">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="15e2e-184">次の検索クエリは、**displayName** または \*emailAddress" に文字「j」で始まる単語がある、`/me` に関連する人物を返します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-184">The following search query returns people relevant to `/me` whose **displayName** or \*emailAddress" has a word that begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

<span data-ttu-id="15e2e-p119">次の例は応答を示しています。既定では、各応答は 10 個のレコードを返します。これは *$top* パラメーターを使用して変更できます。この例では *$top* を使用して 3 つのレコードへの応答を制限しています。</span><span class="sxs-lookup"><span data-stu-id="15e2e-p119">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
      "displayName": "Jan Travis",
      "givenName": "Jan",
      "surname": "Travis",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": "VP Sales",
      "companyName": null,
      "yomiCompany": "",
      "department": "Sales & Marketing",
      "officeLocation": "19/3123",
      "profession": "",
      "userPrincipalName": "JanT@contoso.onmicrosoft.com",
      "imAddress": "sip:JanT@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "JanT@contoso.onmicrosoft.com",
          "relevanceScore": -12.297347783416837
        }
      ],
      "phones": [
        {
          "type": "Business",
          "number": "+1 732 555 0102"
        }
      ],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    },
    {
      "id": "C43BF05E-5B6B-4DCF-B2FC-0837B09E0FA9",
      "displayName": "Jacob Cazares (TAILSPIN)",
      "givenName": null,
      "surname": null,
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": null,
      "companyName": null,
      "yomiCompany": "",
      "department": null,
      "officeLocation": null,
      "profession": "",
      "userPrincipalName": "",
      "imAddress": null,
      "scoredEmailAddresses": [
        {
          "address": "JacobC@tailspintoys.com",
          "relevanceScore": -12.298154282019846
        }
      ],
      "phones": [],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "PersonalContact"
      }
    },
    {
      "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
      "displayName": "Jewell Montgomery",
      "givenName": "Jewell",
      "surname": "Montgomery",
      "birthday": "",
      "personNotes": "",
      "isFavorite": false,
      "jobTitle": null,
      "companyName": null,
      "yomiCompany": "",
      "department": null,
      "officeLocation": null,
      "profession": "",
      "userPrincipalName": "JewellM@contoso.onmicrosoft.com",
      "imAddress": null,
      "scoredEmailAddresses": [
        {
          "address": "JewellM@contoso.onmicrosoft.com",
          "relevanceScore": -12.531408487977451
        }
      ],
      "phones": [],
      "postalAddresses": [],
      "websites": [],
      "personType": {
        "class": "Person",
        "subclass": "OrganizationUser"
      }
    }
  ]
}
```

### <a name="perform-a-fuzzy-search"></a><span data-ttu-id="15e2e-189">あいまい検索の実行</span><span class="sxs-lookup"><span data-stu-id="15e2e-189">Perform a fuzzy search</span></span>

<span data-ttu-id="15e2e-190">検索は、あいまい一致のアルゴリズムを実装します。</span><span class="sxs-lookup"><span data-stu-id="15e2e-190">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="15e2e-191">これにより、完全に一致する項目と、検索目的の推論に基づく結果が返されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-191">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="15e2e-192">たとえば、サインイン ユーザーの **people** コレクションに、表示名が "Tyler Lee" で tylerle@example.com というメール アドレスを持つユーザーがいるとします。</span><span class="sxs-lookup"><span data-stu-id="15e2e-192">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="15e2e-193">次の検索ではすべて、このユーザー Tyler が検索結果として返されます。</span><span class="sxs-lookup"><span data-stu-id="15e2e-193">All of the following searches will return this user Tyler as one of the results.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler"                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle"              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search="tiler"                //fuzzy match with Tyler's name
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"            //matches Tyler's name. Note the quotes to enclose the space.
```
