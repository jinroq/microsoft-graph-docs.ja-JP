---
title: mobileAppCategory の更新
description: mobileAppCategory オブジェクトのプロパティを更新します。
ms.openlocfilehash: cb0e431385a9b8ee21135ac6daf9faf9440f94a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069892"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="ecdc9-103">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="ecdc9-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="ecdc9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecdc9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecdc9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecdc9-107">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecdc9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ecdc9-108">Prerequisites</span></span>
<span data-ttu-id="ecdc9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecdc9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecdc9-111">Permission type</span></span>|<span data-ttu-id="ecdc9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecdc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecdc9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecdc9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecdc9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdc9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecdc9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecdc9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecdc9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-116">Not supported.</span></span>|
|<span data-ttu-id="ecdc9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecdc9-117">Application</span></span>|<span data-ttu-id="ecdc9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecdc9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecdc9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ecdc9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecdc9-120">Request headers</span></span>
|<span data-ttu-id="ecdc9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecdc9-121">Header</span></span>|<span data-ttu-id="ecdc9-122">値</span><span class="sxs-lookup"><span data-stu-id="ecdc9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecdc9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecdc9-123">Authorization</span></span>|<span data-ttu-id="ecdc9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecdc9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecdc9-125">Accept</span></span>|<span data-ttu-id="ecdc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecdc9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecdc9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecdc9-127">Request body</span></span>
<span data-ttu-id="ecdc9-128">要求本文で、[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="ecdc9-129">次の表に、[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="ecdc9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecdc9-130">Property</span></span>|<span data-ttu-id="ecdc9-131">型</span><span class="sxs-lookup"><span data-stu-id="ecdc9-131">Type</span></span>|<span data-ttu-id="ecdc9-132">説明</span><span class="sxs-lookup"><span data-stu-id="ecdc9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecdc9-133">id</span><span class="sxs-lookup"><span data-stu-id="ecdc9-133">id</span></span>|<span data-ttu-id="ecdc9-134">String</span><span class="sxs-lookup"><span data-stu-id="ecdc9-134">String</span></span>|<span data-ttu-id="ecdc9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-135">The key of the entity.</span></span>|
|<span data-ttu-id="ecdc9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ecdc9-136">displayName</span></span>|<span data-ttu-id="ecdc9-137">String</span><span class="sxs-lookup"><span data-stu-id="ecdc9-137">String</span></span>|<span data-ttu-id="ecdc9-138">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-138">The name of the app category.</span></span>|
|<span data-ttu-id="ecdc9-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecdc9-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ecdc9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecdc9-140">DateTimeOffset</span></span>|<span data-ttu-id="ecdc9-141">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ecdc9-142">応答</span><span class="sxs-lookup"><span data-stu-id="ecdc9-142">Response</span></span>
<span data-ttu-id="ecdc9-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecdc9-144">例</span><span class="sxs-lookup"><span data-stu-id="ecdc9-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecdc9-145">要求</span><span class="sxs-lookup"><span data-stu-id="ecdc9-145">Request</span></span>
<span data-ttu-id="ecdc9-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ecdc9-147">応答</span><span class="sxs-lookup"><span data-stu-id="ecdc9-147">Response</span></span>
<span data-ttu-id="ecdc9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ecdc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





