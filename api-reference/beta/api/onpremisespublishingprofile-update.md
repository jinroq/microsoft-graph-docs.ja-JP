---
title: OnPremisesPublishingProfile の更新
description: OnPremisesPublishingProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2cdd2eafc51e5bd38aed41fcfcae259b5a9fe66
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841081"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="3d785-103">OnPremisesPublishingProfile の更新</span><span class="sxs-lookup"><span data-stu-id="3d785-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d785-104">[OnPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3d785-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d785-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d785-105">Permissions</span></span>

<span data-ttu-id="3d785-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d785-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d785-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d785-108">Permission type</span></span>                        | <span data-ttu-id="3d785-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d785-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="3d785-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d785-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d785-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="3d785-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="3d785-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d785-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d785-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d785-113">Not supported.</span></span> |
| <span data-ttu-id="3d785-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d785-114">Application</span></span>                            | <span data-ttu-id="3d785-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d785-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d785-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d785-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="3d785-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d785-117">Request headers</span></span>

| <span data-ttu-id="3d785-118">名前</span><span class="sxs-lookup"><span data-stu-id="3d785-118">Name</span></span>       | <span data-ttu-id="3d785-119">説明</span><span class="sxs-lookup"><span data-stu-id="3d785-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3d785-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d785-120">Authorization</span></span> | <span data-ttu-id="3d785-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="3d785-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d785-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d785-122">Request body</span></span>

<span data-ttu-id="3d785-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d785-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="3d785-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="3d785-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3d785-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3d785-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d785-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d785-126">Property</span></span>     | <span data-ttu-id="3d785-127">型</span><span class="sxs-lookup"><span data-stu-id="3d785-127">Type</span></span>        | <span data-ttu-id="3d785-128">説明</span><span class="sxs-lookup"><span data-stu-id="3d785-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d785-129">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d785-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="3d785-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d785-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="3d785-131">[HybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="3d785-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3d785-132">応答</span><span class="sxs-lookup"><span data-stu-id="3d785-132">Response</span></span>

<span data-ttu-id="3d785-133">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3d785-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3d785-134">例</span><span class="sxs-lookup"><span data-stu-id="3d785-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3d785-135">例 1: hybridAgentUpdaterConfiguration の [更新プログラムの更新] ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="3d785-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="3d785-136">次の例では、 **hybridAgentUpdaterConfiguration**の**updatewindow**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3d785-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3d785-137">要求</span><span class="sxs-lookup"><span data-stu-id="3d785-137">Request</span></span>

<span data-ttu-id="3d785-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d785-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3d785-139">応答</span><span class="sxs-lookup"><span data-stu-id="3d785-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3d785-140">例 2: hybridAgentUpdaterConfiguration で deferUpdate を更新する</span><span class="sxs-lookup"><span data-stu-id="3d785-140">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="3d785-141">次の例では、 **hybridAgentUpdaterConfiguration**の**deferUpdate**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3d785-141">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3d785-142">要求</span><span class="sxs-lookup"><span data-stu-id="3d785-142">Request</span></span>

<span data-ttu-id="3d785-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d785-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3d785-144">応答</span><span class="sxs-lookup"><span data-stu-id="3d785-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="3d785-145">例 3: hybridAgentUpdaterConfiguration で allowUpdateConfigurationOverride を更新する</span><span class="sxs-lookup"><span data-stu-id="3d785-145">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="3d785-146">次の例では、 **hybridAgentUpdaterConfiguration**の**allowUpdateConfigurationOverride**を更新します。</span><span class="sxs-lookup"><span data-stu-id="3d785-146">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="3d785-147">要求</span><span class="sxs-lookup"><span data-stu-id="3d785-147">Request</span></span>

<span data-ttu-id="3d785-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d785-148">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3d785-149">応答</span><span class="sxs-lookup"><span data-stu-id="3d785-149">Response</span></span>

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
