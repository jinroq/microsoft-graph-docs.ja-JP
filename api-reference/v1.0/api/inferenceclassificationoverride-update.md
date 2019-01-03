---
title: inferenceClassificationOverride を更新する
description: '指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。 '
ms.openlocfilehash: c88b750275a1a3c52edf356ecd93a5c3ba6a3770
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021641"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="8926c-103">inferenceClassificationOverride を更新する</span><span class="sxs-lookup"><span data-stu-id="8926c-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="8926c-104">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="8926c-104">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="8926c-105">[InferenceClassicationOverride](../resources/inferenceclassificationoverride.md) インスタンスのその他のフィールドの変更には、PATCH を使用できません。</span><span class="sxs-lookup"><span data-stu-id="8926c-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="8926c-106">送信者にオーバーライドがあり、その送信者が表示名を変更すると、既存のオーバーライドで [POST](inferenceclassification-post-overrides.md) を使用して [名前] フィールドの更新を実施できます。</span><span class="sxs-lookup"><span data-stu-id="8926c-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="8926c-107">送信者にオーバーライドがあり、その送信者が SMTP アドレスを変更すると、既存のオーバーライドを[削除](inferenceclassificationoverride-delete.md)して、新しい SMTP アドレスで新しくオーバーライドを[作成](inferenceclassification-post-overrides.md)することが、この送信者のオーバーライドを「更新」する唯一の方法になります。</span><span class="sxs-lookup"><span data-stu-id="8926c-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="8926c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8926c-108">Permissions</span></span>
<span data-ttu-id="8926c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8926c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8926c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8926c-111">Permission type</span></span>      | <span data-ttu-id="8926c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8926c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8926c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8926c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8926c-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8926c-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8926c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8926c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8926c-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8926c-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8926c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8926c-117">Application</span></span> | <span data-ttu-id="8926c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8926c-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8926c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8926c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8926c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8926c-120">Request headers</span></span>
| <span data-ttu-id="8926c-121">名前</span><span class="sxs-lookup"><span data-stu-id="8926c-121">Name</span></span>       | <span data-ttu-id="8926c-122">型</span><span class="sxs-lookup"><span data-stu-id="8926c-122">Type</span></span> | <span data-ttu-id="8926c-123">説明</span><span class="sxs-lookup"><span data-stu-id="8926c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8926c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8926c-124">Authorization</span></span>  | <span data-ttu-id="8926c-125">string</span><span class="sxs-lookup"><span data-stu-id="8926c-125">string</span></span>  | <span data-ttu-id="8926c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8926c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8926c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8926c-128">Content-Type</span></span> | <span data-ttu-id="8926c-129">string</span><span class="sxs-lookup"><span data-stu-id="8926c-129">string</span></span>  | <span data-ttu-id="8926c-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="8926c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8926c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="8926c-132">Request body</span></span>
<span data-ttu-id="8926c-p104">要求の本文内に、**classifyAs** の新しい値を指定します。最適なパフォーマンスを得るためには、変更されない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8926c-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="8926c-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8926c-135">Property</span></span>     | <span data-ttu-id="8926c-136">型</span><span class="sxs-lookup"><span data-stu-id="8926c-136">Type</span></span>   |<span data-ttu-id="8926c-137">説明</span><span class="sxs-lookup"><span data-stu-id="8926c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8926c-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="8926c-138">classifyAs</span></span>|<span data-ttu-id="8926c-139">文字列</span><span class="sxs-lookup"><span data-stu-id="8926c-139">string</span></span>| <span data-ttu-id="8926c-140">特定の差出人からの着信メッセージを常時分類する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="8926c-140">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="8926c-141">可能な値: `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="8926c-141">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="8926c-142">応答</span><span class="sxs-lookup"><span data-stu-id="8926c-142">Response</span></span>

<span data-ttu-id="8926c-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8926c-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8926c-144">例</span><span class="sxs-lookup"><span data-stu-id="8926c-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8926c-145">要求</span><span class="sxs-lookup"><span data-stu-id="8926c-145">Request</span></span>
<span data-ttu-id="8926c-146">以下の例は、SMTP アドレス randiw@adatum.onmicrosoft.com のオーバーライドのものであり、`other` から `focused` に変更します。</span><span class="sxs-lookup"><span data-stu-id="8926c-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="8926c-147">応答</span><span class="sxs-lookup"><span data-stu-id="8926c-147">Response</span></span>
<span data-ttu-id="8926c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8926c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->