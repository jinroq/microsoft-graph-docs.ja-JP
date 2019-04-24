---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'この関数は、すべてのファイルベースのリソース (Word、Excel など) をアップロードする必要がある OneDrive の URL を返します。  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 43bef729d2cf37561d0742ebb3adfb21fe4f486e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464654"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="959dc-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="959dc-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="959dc-104">この関数は、すべてのファイルベースのリソース (Word、Excel など) をアップロードする必要がある OneDrive の URL を返します。</span><span class="sxs-lookup"><span data-stu-id="959dc-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="959dc-105">リソースとして追加するためには、ファイルをこのフォルダーに配置する必要がありますのでご注意ください。</span><span class="sxs-lookup"><span data-stu-id="959dc-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="959dc-106">クラス内の教師のみが、アップロードするファイルを決定できます。</span><span class="sxs-lookup"><span data-stu-id="959dc-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="959dc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="959dc-107">Permissions</span></span>
<span data-ttu-id="959dc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="959dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="959dc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="959dc-110">Permission type</span></span>      | <span data-ttu-id="959dc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="959dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="959dc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="959dc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="959dc-113">EduAssignments (basic、EduAssignments)</span><span class="sxs-lookup"><span data-stu-id="959dc-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="959dc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="959dc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="959dc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="959dc-115">Not supported.</span></span>  |
|<span data-ttu-id="959dc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="959dc-116">Application</span></span> | <span data-ttu-id="959dc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="959dc-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="959dc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="959dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="959dc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="959dc-119">Request headers</span></span>
| <span data-ttu-id="959dc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="959dc-120">Header</span></span>       | <span data-ttu-id="959dc-121">値</span><span class="sxs-lookup"><span data-stu-id="959dc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="959dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="959dc-122">Authorization</span></span>  | <span data-ttu-id="959dc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="959dc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="959dc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="959dc-125">Request body</span></span>
<span data-ttu-id="959dc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="959dc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="959dc-127">応答</span><span class="sxs-lookup"><span data-stu-id="959dc-127">Response</span></span>
<span data-ttu-id="959dc-128">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="959dc-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="959dc-129">本文には、すべてのファイルベースのリソースを格納するフォルダーの OneDrive URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="959dc-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="959dc-130">例</span><span class="sxs-lookup"><span data-stu-id="959dc-130">Example</span></span>
<span data-ttu-id="959dc-131">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="959dc-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="959dc-132">要求</span><span class="sxs-lookup"><span data-stu-id="959dc-132">Request</span></span>
<span data-ttu-id="959dc-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="959dc-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="959dc-134">応答</span><span class="sxs-lookup"><span data-stu-id="959dc-134">Response</span></span>
<span data-ttu-id="959dc-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="959dc-135">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
