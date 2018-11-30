---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'この関数は、すべてのファイルベースのリソース (Word、Excel、およびなど) をアップロードする必要があります OneDrive の URL を返します。  '
ms.openlocfilehash: 129fa76d57e2016141397f967e833c765e737b19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071394"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="60320-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="60320-103">educationAssignment: getResourcesFolderUrl</span></span>

> <span data-ttu-id="60320-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60320-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60320-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60320-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60320-106">この関数は、すべてのファイルベースのリソース (Word、Excel、およびなど) をアップロードする必要があります OneDrive の URL を返します。</span><span class="sxs-lookup"><span data-stu-id="60320-106">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="60320-107">ファイルをリソースとして追加するためにこのフォルダーに配置する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="60320-107">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="60320-108">クラスの先生だけでは、アップロードするファイルを確認できます。</span><span class="sxs-lookup"><span data-stu-id="60320-108">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="60320-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60320-109">Permissions</span></span>
<span data-ttu-id="60320-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60320-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60320-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60320-112">Permission type</span></span>      | <span data-ttu-id="60320-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60320-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60320-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60320-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="60320-115">EduAssignments.ReadBasic、EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="60320-115">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="60320-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60320-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="60320-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60320-117">Not supported.</span></span>  |
|<span data-ttu-id="60320-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60320-118">Application</span></span> | <span data-ttu-id="60320-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60320-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="60320-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60320-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="60320-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60320-121">Request headers</span></span>
| <span data-ttu-id="60320-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60320-122">Header</span></span>       | <span data-ttu-id="60320-123">値</span><span class="sxs-lookup"><span data-stu-id="60320-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60320-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="60320-124">Authorization</span></span>  | <span data-ttu-id="60320-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60320-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60320-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="60320-127">Request body</span></span>
<span data-ttu-id="60320-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60320-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="60320-129">応答</span><span class="sxs-lookup"><span data-stu-id="60320-129">Response</span></span>
<span data-ttu-id="60320-130">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="60320-130">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="60320-131">本体ですべてのファイル ・ ベースのリソースが格納されるフォルダーの OneDrive の URL が含まれます。</span><span class="sxs-lookup"><span data-stu-id="60320-131">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="60320-132">例</span><span class="sxs-lookup"><span data-stu-id="60320-132">Example</span></span>
<span data-ttu-id="60320-133">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="60320-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60320-134">要求</span><span class="sxs-lookup"><span data-stu-id="60320-134">Request</span></span>
<span data-ttu-id="60320-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60320-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="60320-136">応答</span><span class="sxs-lookup"><span data-stu-id="60320-136">Response</span></span>
<span data-ttu-id="60320-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60320-137">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
