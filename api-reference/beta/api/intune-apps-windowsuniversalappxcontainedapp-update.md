---
title: WindowsUniversalAppXContainedApp の更新
description: WindowsUniversalAppXContainedApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 172828ebe237ae076274f487826584ed43d2756f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959580"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="c15e8-103">WindowsUniversalAppXContainedApp の更新</span><span class="sxs-lookup"><span data-stu-id="c15e8-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="c15e8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c15e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c15e8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c15e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c15e8-106">[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c15e8-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c15e8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c15e8-107">Prerequisites</span></span>
<span data-ttu-id="c15e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c15e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c15e8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c15e8-110">Permission type</span></span>|<span data-ttu-id="c15e8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c15e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c15e8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c15e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c15e8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c15e8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c15e8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c15e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c15e8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c15e8-115">Not supported.</span></span>|
|<span data-ttu-id="c15e8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c15e8-116">Application</span></span>|<span data-ttu-id="c15e8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c15e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c15e8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c15e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c15e8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c15e8-119">Request headers</span></span>
|<span data-ttu-id="c15e8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c15e8-120">Header</span></span>|<span data-ttu-id="c15e8-121">値</span><span class="sxs-lookup"><span data-stu-id="c15e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c15e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c15e8-122">Authorization</span></span>|<span data-ttu-id="c15e8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c15e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c15e8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c15e8-124">Accept</span></span>|<span data-ttu-id="c15e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c15e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c15e8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c15e8-126">Request body</span></span>
<span data-ttu-id="c15e8-127">要求本文で、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c15e8-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="c15e8-128">次の表に、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c15e8-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="c15e8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c15e8-129">Property</span></span>|<span data-ttu-id="c15e8-130">型</span><span class="sxs-lookup"><span data-stu-id="c15e8-130">Type</span></span>|<span data-ttu-id="c15e8-131">説明</span><span class="sxs-lookup"><span data-stu-id="c15e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c15e8-132">id</span><span class="sxs-lookup"><span data-stu-id="c15e8-132">id</span></span>|<span data-ttu-id="c15e8-133">String</span><span class="sxs-lookup"><span data-stu-id="c15e8-133">String</span></span>|<span data-ttu-id="c15e8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c15e8-134">Key of the entity.</span></span> <span data-ttu-id="c15e8-135">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c15e8-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c15e8-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c15e8-136">appUserModelId</span></span>|<span data-ttu-id="c15e8-137">String</span><span class="sxs-lookup"><span data-stu-id="c15e8-137">String</span></span>|<span data-ttu-id="c15e8-138">WindowsUniversalAppX アプリの含まれているアプリのアプリユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="c15e8-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="c15e8-139">応答</span><span class="sxs-lookup"><span data-stu-id="c15e8-139">Response</span></span>
<span data-ttu-id="c15e8-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c15e8-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c15e8-141">例</span><span class="sxs-lookup"><span data-stu-id="c15e8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c15e8-142">要求</span><span class="sxs-lookup"><span data-stu-id="c15e8-142">Request</span></span>
<span data-ttu-id="c15e8-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c15e8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c15e8-144">応答</span><span class="sxs-lookup"><span data-stu-id="c15e8-144">Response</span></span>
<span data-ttu-id="c15e8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c15e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





