---
title: DataPolicyOperation を取得します。
description: DataPolicyOperation オブジェクトのプロパティを取得します。
ms.openlocfilehash: fbc94719f9944adb25f7dd744cf0b15b179f3a5d
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156020"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="7bdbc-103">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="7bdbc-104">DataPolicyOperation オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bdbc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7bdbc-105">Permissions</span></span>
<span data-ttu-id="7bdbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bdbc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bdbc-108">Permission type</span></span>      | <span data-ttu-id="7bdbc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bdbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bdbc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bdbc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7bdbc-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7bdbc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7bdbc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bdbc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7bdbc-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="7bdbc-113">Not applicable</span></span>  |
|<span data-ttu-id="7bdbc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bdbc-114">Application</span></span> | <span data-ttu-id="7bdbc-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bdbc-115">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7bdbc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bdbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7bdbc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bdbc-117">Request headers</span></span>
| <span data-ttu-id="7bdbc-118">名前</span><span class="sxs-lookup"><span data-stu-id="7bdbc-118">Name</span></span>      |<span data-ttu-id="7bdbc-119">説明</span><span class="sxs-lookup"><span data-stu-id="7bdbc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bdbc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bdbc-120">Authorization</span></span>  | <span data-ttu-id="7bdbc-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="7bdbc-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bdbc-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bdbc-122">Request body</span></span>
<span data-ttu-id="7bdbc-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7bdbc-124">応答</span><span class="sxs-lookup"><span data-stu-id="7bdbc-124">Response</span></span>
<span data-ttu-id="7bdbc-125">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[dataPolicyOperation](../resources/datapolicyoperation.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bdbc-126">例</span><span class="sxs-lookup"><span data-stu-id="7bdbc-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bdbc-127">要求</span><span class="sxs-lookup"><span data-stu-id="7bdbc-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="7bdbc-128">応答</span><span class="sxs-lookup"><span data-stu-id="7bdbc-128">Response</span></span>
<span data-ttu-id="7bdbc-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7bdbc-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "progress-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
