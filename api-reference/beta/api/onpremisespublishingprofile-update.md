---
title: OnPremisesPublishingProfile の更新
description: OnPremisesPublishingProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b4d2eac82b47549633b03c39465e4107e4fcd8b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414503"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="3629a-103">OnPremisesPublishingProfile の更新</span><span class="sxs-lookup"><span data-stu-id="3629a-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3629a-104">[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3629a-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3629a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3629a-105">Permissions</span></span>

<span data-ttu-id="3629a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3629a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3629a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3629a-108">Permission type</span></span>                        | <span data-ttu-id="3629a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3629a-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="3629a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3629a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3629a-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="3629a-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="3629a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3629a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3629a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3629a-113">Not supported.</span></span> |
| <span data-ttu-id="3629a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3629a-114">Application</span></span>                            | <span data-ttu-id="3629a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3629a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3629a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3629a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="3629a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3629a-117">Request headers</span></span>

| <span data-ttu-id="3629a-118">名前</span><span class="sxs-lookup"><span data-stu-id="3629a-118">Name</span></span>       | <span data-ttu-id="3629a-119">説明</span><span class="sxs-lookup"><span data-stu-id="3629a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3629a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3629a-120">Authorization</span></span> | <span data-ttu-id="3629a-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="3629a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3629a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="3629a-122">Request body</span></span>

<span data-ttu-id="3629a-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3629a-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="3629a-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="3629a-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3629a-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3629a-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3629a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3629a-126">Property</span></span>     | <span data-ttu-id="3629a-127">型</span><span class="sxs-lookup"><span data-stu-id="3629a-127">Type</span></span>        | <span data-ttu-id="3629a-128">説明</span><span class="sxs-lookup"><span data-stu-id="3629a-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3629a-129">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="3629a-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="3629a-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="3629a-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="3629a-131">[HybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="3629a-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3629a-132">応答</span><span class="sxs-lookup"><span data-stu-id="3629a-132">Response</span></span>

<span data-ttu-id="3629a-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3629a-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3629a-134">例</span><span class="sxs-lookup"><span data-stu-id="3629a-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3629a-135">例 1: hybridAgentUpdaterConfiguration の [更新プログラムの更新] ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="3629a-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="3629a-136">次の例では、 **hybridAgentUpdaterConfiguration**の**updatewindow**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3629a-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3629a-137">要求</span><span class="sxs-lookup"><span data-stu-id="3629a-137">Request</span></span>

<span data-ttu-id="3629a-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3629a-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3629a-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3629a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3629a-140">C#</span><span class="sxs-lookup"><span data-stu-id="3629a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3629a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3629a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3629a-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="3629a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3629a-143">応答</span><span class="sxs-lookup"><span data-stu-id="3629a-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3629a-144">例 2: hybridAgentUpdaterConfiguration で deferUpdate を更新する</span><span class="sxs-lookup"><span data-stu-id="3629a-144">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="3629a-145">次の例では、 **hybridAgentUpdaterConfiguration**の**deferUpdate**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3629a-145">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3629a-146">要求</span><span class="sxs-lookup"><span data-stu-id="3629a-146">Request</span></span>

<span data-ttu-id="3629a-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3629a-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="3629a-148">応答</span><span class="sxs-lookup"><span data-stu-id="3629a-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3629a-149">例 3: hybridAgentUpdaterConfiguration で allowUpdateConfigurationOverride を更新する</span><span class="sxs-lookup"><span data-stu-id="3629a-149">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="3629a-150">次の例では、 **hybridAgentUpdaterConfiguration**の**allowUpdateConfigurationOverride**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3629a-150">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3629a-151">要求</span><span class="sxs-lookup"><span data-stu-id="3629a-151">Request</span></span>

<span data-ttu-id="3629a-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3629a-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="3629a-153">応答</span><span class="sxs-lookup"><span data-stu-id="3629a-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
