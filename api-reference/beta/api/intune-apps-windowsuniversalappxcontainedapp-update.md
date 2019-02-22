---
title: windowsUniversalAppXContainedApp の更新
description: windowsUniversalAppXContainedApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a3bacf74734fefe8255da981f0f71f4389db610
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159837"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="c9262-103">windowsUniversalAppXContainedApp の更新</span><span class="sxs-lookup"><span data-stu-id="c9262-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="c9262-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9262-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9262-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9262-106">[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c9262-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9262-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9262-107">Prerequisites</span></span>
<span data-ttu-id="c9262-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9262-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9262-110">Permission type</span></span>|<span data-ttu-id="c9262-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9262-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9262-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9262-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9262-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9262-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9262-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9262-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9262-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9262-115">Not supported.</span></span>|
|<span data-ttu-id="c9262-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9262-116">Application</span></span>|<span data-ttu-id="c9262-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9262-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9262-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9262-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c9262-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9262-119">Request headers</span></span>
|<span data-ttu-id="c9262-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9262-120">Header</span></span>|<span data-ttu-id="c9262-121">値</span><span class="sxs-lookup"><span data-stu-id="c9262-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9262-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9262-122">Authorization</span></span>|<span data-ttu-id="c9262-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c9262-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9262-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c9262-124">Accept</span></span>|<span data-ttu-id="c9262-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9262-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9262-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9262-126">Request body</span></span>
<span data-ttu-id="c9262-127">要求本文で、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9262-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="c9262-128">次の表に、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c9262-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="c9262-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9262-129">Property</span></span>|<span data-ttu-id="c9262-130">型</span><span class="sxs-lookup"><span data-stu-id="c9262-130">Type</span></span>|<span data-ttu-id="c9262-131">説明</span><span class="sxs-lookup"><span data-stu-id="c9262-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9262-132">id</span><span class="sxs-lookup"><span data-stu-id="c9262-132">id</span></span>|<span data-ttu-id="c9262-133">String</span><span class="sxs-lookup"><span data-stu-id="c9262-133">String</span></span>|<span data-ttu-id="c9262-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c9262-134">Key of the entity.</span></span> <span data-ttu-id="c9262-135">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9262-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c9262-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c9262-136">appUserModelId</span></span>|<span data-ttu-id="c9262-137">String</span><span class="sxs-lookup"><span data-stu-id="c9262-137">String</span></span>|<span data-ttu-id="c9262-138">WindowsUniversalAppX アプリの含まれているアプリのアプリユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="c9262-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="c9262-139">応答</span><span class="sxs-lookup"><span data-stu-id="c9262-139">Response</span></span>
<span data-ttu-id="c9262-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9262-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9262-141">例</span><span class="sxs-lookup"><span data-stu-id="c9262-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9262-142">要求</span><span class="sxs-lookup"><span data-stu-id="c9262-142">Request</span></span>
<span data-ttu-id="c9262-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9262-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c9262-144">応答</span><span class="sxs-lookup"><span data-stu-id="c9262-144">Response</span></span>
<span data-ttu-id="c9262-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9262-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




