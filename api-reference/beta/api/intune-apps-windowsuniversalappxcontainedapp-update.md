---
title: WindowsUniversalAppXContainedApp の更新
description: WindowsUniversalAppXContainedApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2f3748c17a1bfabe48210e4fb83c110580a07e4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934419"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="ecfc7-103">WindowsUniversalAppXContainedApp の更新</span><span class="sxs-lookup"><span data-stu-id="ecfc7-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="ecfc7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecfc7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecfc7-106">[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecfc7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ecfc7-107">Prerequisites</span></span>
<span data-ttu-id="ecfc7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecfc7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecfc7-110">Permission type</span></span>|<span data-ttu-id="ecfc7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecfc7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecfc7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecfc7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecfc7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecfc7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecfc7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecfc7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecfc7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-115">Not supported.</span></span>|
|<span data-ttu-id="ecfc7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecfc7-116">Application</span></span>|<span data-ttu-id="ecfc7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecfc7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecfc7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ecfc7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecfc7-119">Request headers</span></span>
|<span data-ttu-id="ecfc7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecfc7-120">Header</span></span>|<span data-ttu-id="ecfc7-121">値</span><span class="sxs-lookup"><span data-stu-id="ecfc7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecfc7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecfc7-122">Authorization</span></span>|<span data-ttu-id="ecfc7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecfc7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ecfc7-124">Accept</span></span>|<span data-ttu-id="ecfc7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecfc7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecfc7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecfc7-126">Request body</span></span>
<span data-ttu-id="ecfc7-127">要求本文で、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="ecfc7-128">次の表に、 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="ecfc7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecfc7-129">Property</span></span>|<span data-ttu-id="ecfc7-130">型</span><span class="sxs-lookup"><span data-stu-id="ecfc7-130">Type</span></span>|<span data-ttu-id="ecfc7-131">説明</span><span class="sxs-lookup"><span data-stu-id="ecfc7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecfc7-132">id</span><span class="sxs-lookup"><span data-stu-id="ecfc7-132">id</span></span>|<span data-ttu-id="ecfc7-133">String</span><span class="sxs-lookup"><span data-stu-id="ecfc7-133">String</span></span>|<span data-ttu-id="ecfc7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-134">Key of the entity.</span></span> <span data-ttu-id="ecfc7-135">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="ecfc7-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="ecfc7-136">appUserModelId</span></span>|<span data-ttu-id="ecfc7-137">String</span><span class="sxs-lookup"><span data-stu-id="ecfc7-137">String</span></span>|<span data-ttu-id="ecfc7-138">WindowsUniversalAppX アプリの含まれているアプリのアプリユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="ecfc7-139">応答</span><span class="sxs-lookup"><span data-stu-id="ecfc7-139">Response</span></span>
<span data-ttu-id="ecfc7-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecfc7-141">例</span><span class="sxs-lookup"><span data-stu-id="ecfc7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecfc7-142">要求</span><span class="sxs-lookup"><span data-stu-id="ecfc7-142">Request</span></span>
<span data-ttu-id="ecfc7-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="ecfc7-144">応答</span><span class="sxs-lookup"><span data-stu-id="ecfc7-144">Response</span></span>
<span data-ttu-id="ecfc7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ecfc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




