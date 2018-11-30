---
title: MicrosoftStoreForBusinessContainedApp を作成します。
description: 新しい microsoftStoreForBusinessContainedApp オブジェクトを作成します。
ms.openlocfilehash: 131e510a1526879ffcb94c3782d9fa263dd4645c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068620"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="101e0-103">MicrosoftStoreForBusinessContainedApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="101e0-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="101e0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="101e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="101e0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="101e0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="101e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="101e0-107">新しい[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="101e0-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="101e0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="101e0-108">Prerequisites</span></span>
<span data-ttu-id="101e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="101e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="101e0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="101e0-111">Permission type</span></span>|<span data-ttu-id="101e0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="101e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="101e0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="101e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="101e0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="101e0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="101e0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="101e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="101e0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101e0-116">Not supported.</span></span>|
|<span data-ttu-id="101e0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="101e0-117">Application</span></span>|<span data-ttu-id="101e0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="101e0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="101e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="101e0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="101e0-120">Request headers</span></span>
|<span data-ttu-id="101e0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="101e0-121">Header</span></span>|<span data-ttu-id="101e0-122">値</span><span class="sxs-lookup"><span data-stu-id="101e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="101e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="101e0-123">Authorization</span></span>|<span data-ttu-id="101e0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="101e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="101e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="101e0-125">Accept</span></span>|<span data-ttu-id="101e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="101e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="101e0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="101e0-127">Request body</span></span>
<span data-ttu-id="101e0-128">要求の本文に microsoftStoreForBusinessContainedApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="101e0-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="101e0-129">次の表は、microsoftStoreForBusinessContainedApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="101e0-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="101e0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="101e0-130">Property</span></span>|<span data-ttu-id="101e0-131">型</span><span class="sxs-lookup"><span data-stu-id="101e0-131">Type</span></span>|<span data-ttu-id="101e0-132">説明</span><span class="sxs-lookup"><span data-stu-id="101e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="101e0-133">id</span><span class="sxs-lookup"><span data-stu-id="101e0-133">id</span></span>|<span data-ttu-id="101e0-134">String</span><span class="sxs-lookup"><span data-stu-id="101e0-134">String</span></span>|<span data-ttu-id="101e0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="101e0-135">Key of the entity.</span></span> <span data-ttu-id="101e0-136">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="101e0-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="101e0-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="101e0-137">appUserModelId</span></span>|<span data-ttu-id="101e0-138">String</span><span class="sxs-lookup"><span data-stu-id="101e0-138">String</span></span>|<span data-ttu-id="101e0-139">MicrosoftStoreForBusinessApp の格納されているアプリケーションのアプリケーション ユーザー モデル ID です。</span><span class="sxs-lookup"><span data-stu-id="101e0-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="101e0-140">応答</span><span class="sxs-lookup"><span data-stu-id="101e0-140">Response</span></span>
<span data-ttu-id="101e0-141">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="101e0-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="101e0-142">例</span><span class="sxs-lookup"><span data-stu-id="101e0-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="101e0-143">要求</span><span class="sxs-lookup"><span data-stu-id="101e0-143">Request</span></span>
<span data-ttu-id="101e0-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="101e0-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="101e0-145">応答</span><span class="sxs-lookup"><span data-stu-id="101e0-145">Response</span></span>
<span data-ttu-id="101e0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="101e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





