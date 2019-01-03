---
title: mobileAppCategory の作成
description: 新しい mobileAppCategory オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 7fa2b8220069dd98ec35124f589a3e38a2a33317
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330948"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="3a0ea-103">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="3a0ea-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="3a0ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a0ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a0ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a0ea-107">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a0ea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3a0ea-108">Prerequisites</span></span>
<span data-ttu-id="3a0ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a0ea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a0ea-111">Permission type</span></span>|<span data-ttu-id="3a0ea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a0ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a0ea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a0ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a0ea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a0ea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a0ea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a0ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a0ea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-116">Not supported.</span></span>|
|<span data-ttu-id="3a0ea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a0ea-117">Application</span></span>|<span data-ttu-id="3a0ea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a0ea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a0ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="3a0ea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a0ea-120">Request headers</span></span>
|<span data-ttu-id="3a0ea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a0ea-121">Header</span></span>|<span data-ttu-id="3a0ea-122">値</span><span class="sxs-lookup"><span data-stu-id="3a0ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a0ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a0ea-123">Authorization</span></span>|<span data-ttu-id="3a0ea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a0ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a0ea-125">Accept</span></span>|<span data-ttu-id="3a0ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a0ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a0ea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a0ea-127">Request body</span></span>
<span data-ttu-id="3a0ea-128">要求本文で、mobileAppCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="3a0ea-129">次の表に、mobileAppCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="3a0ea-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a0ea-130">Property</span></span>|<span data-ttu-id="3a0ea-131">種類</span><span class="sxs-lookup"><span data-stu-id="3a0ea-131">Type</span></span>|<span data-ttu-id="3a0ea-132">説明</span><span class="sxs-lookup"><span data-stu-id="3a0ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a0ea-133">ID</span><span class="sxs-lookup"><span data-stu-id="3a0ea-133">id</span></span>|<span data-ttu-id="3a0ea-134">String</span><span class="sxs-lookup"><span data-stu-id="3a0ea-134">String</span></span>|<span data-ttu-id="3a0ea-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-135">The key of the entity.</span></span>|
|<span data-ttu-id="3a0ea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3a0ea-136">displayName</span></span>|<span data-ttu-id="3a0ea-137">String</span><span class="sxs-lookup"><span data-stu-id="3a0ea-137">String</span></span>|<span data-ttu-id="3a0ea-138">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-138">The name of the app category.</span></span>|
|<span data-ttu-id="3a0ea-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a0ea-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3a0ea-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a0ea-140">DateTimeOffset</span></span>|<span data-ttu-id="3a0ea-141">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3a0ea-142">応答</span><span class="sxs-lookup"><span data-stu-id="3a0ea-142">Response</span></span>
<span data-ttu-id="3a0ea-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a0ea-144">例</span><span class="sxs-lookup"><span data-stu-id="3a0ea-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a0ea-145">要求</span><span class="sxs-lookup"><span data-stu-id="3a0ea-145">Request</span></span>
<span data-ttu-id="3a0ea-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3a0ea-147">応答</span><span class="sxs-lookup"><span data-stu-id="3a0ea-147">Response</span></span>
<span data-ttu-id="3a0ea-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a0ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




