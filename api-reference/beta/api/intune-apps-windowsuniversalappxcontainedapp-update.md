---
title: WindowsUniversalAppXContainedApp を更新します。
description: WindowsUniversalAppXContainedApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: f39046e10917a45ba880777992247748e89a24e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339110"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="1a079-103">WindowsUniversalAppXContainedApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="1a079-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="1a079-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a079-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a079-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a079-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a079-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a079-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a079-107">[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a079-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a079-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a079-108">Prerequisites</span></span>
<span data-ttu-id="1a079-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a079-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a079-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a079-111">Permission type</span></span>|<span data-ttu-id="1a079-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a079-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a079-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a079-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a079-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a079-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a079-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a079-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a079-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a079-116">Not supported.</span></span>|
|<span data-ttu-id="1a079-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a079-117">Application</span></span>|<span data-ttu-id="1a079-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a079-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a079-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a079-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1a079-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a079-120">Request headers</span></span>
|<span data-ttu-id="1a079-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a079-121">Header</span></span>|<span data-ttu-id="1a079-122">値</span><span class="sxs-lookup"><span data-stu-id="1a079-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a079-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a079-123">Authorization</span></span>|<span data-ttu-id="1a079-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a079-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a079-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a079-125">Accept</span></span>|<span data-ttu-id="1a079-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a079-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a079-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a079-127">Request body</span></span>
<span data-ttu-id="1a079-128">要求の本文に[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a079-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="1a079-129">[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="1a079-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="1a079-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a079-130">Property</span></span>|<span data-ttu-id="1a079-131">種類</span><span class="sxs-lookup"><span data-stu-id="1a079-131">Type</span></span>|<span data-ttu-id="1a079-132">説明</span><span class="sxs-lookup"><span data-stu-id="1a079-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a079-133">ID</span><span class="sxs-lookup"><span data-stu-id="1a079-133">id</span></span>|<span data-ttu-id="1a079-134">String</span><span class="sxs-lookup"><span data-stu-id="1a079-134">String</span></span>|<span data-ttu-id="1a079-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a079-135">Key of the entity.</span></span> <span data-ttu-id="1a079-136">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1a079-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="1a079-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="1a079-137">appUserModelId</span></span>|<span data-ttu-id="1a079-138">String</span><span class="sxs-lookup"><span data-stu-id="1a079-138">String</span></span>|<span data-ttu-id="1a079-139">WindowsUniversalAppX アプリケーションの格納されているアプリケーションのアプリケーション ユーザー モデル ID です。</span><span class="sxs-lookup"><span data-stu-id="1a079-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="1a079-140">応答</span><span class="sxs-lookup"><span data-stu-id="1a079-140">Response</span></span>
<span data-ttu-id="1a079-141">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1a079-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a079-142">例</span><span class="sxs-lookup"><span data-stu-id="1a079-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a079-143">要求</span><span class="sxs-lookup"><span data-stu-id="1a079-143">Request</span></span>
<span data-ttu-id="1a079-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a079-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="1a079-145">応答</span><span class="sxs-lookup"><span data-stu-id="1a079-145">Response</span></span>
<span data-ttu-id="1a079-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a079-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```





