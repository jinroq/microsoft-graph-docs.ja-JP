---
title: windowsUniversalAppXContainedApp を作成する
description: 新しい windowsUniversalAppXContainedApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c60644e72a5885a2155ed8ef9feae965bd86b0cb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780848"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="0f566-103">windowsUniversalAppXContainedApp を作成する</span><span class="sxs-lookup"><span data-stu-id="0f566-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="0f566-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f566-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f566-106">新しい[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f566-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f566-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f566-107">Prerequisites</span></span>
<span data-ttu-id="0f566-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f566-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f566-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f566-110">Permission type</span></span>|<span data-ttu-id="0f566-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f566-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f566-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f566-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f566-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f566-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f566-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f566-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f566-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f566-115">Not supported.</span></span>|
|<span data-ttu-id="0f566-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f566-116">Application</span></span>|<span data-ttu-id="0f566-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f566-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f566-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f566-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="0f566-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f566-119">Request headers</span></span>
|<span data-ttu-id="0f566-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f566-120">Header</span></span>|<span data-ttu-id="0f566-121">値</span><span class="sxs-lookup"><span data-stu-id="0f566-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f566-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f566-122">Authorization</span></span>|<span data-ttu-id="0f566-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f566-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f566-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0f566-124">Accept</span></span>|<span data-ttu-id="0f566-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f566-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f566-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f566-126">Request body</span></span>
<span data-ttu-id="0f566-127">要求本文で、windowsUniversalAppXContainedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f566-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="0f566-128">次の表に、windowsUniversalAppXContainedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f566-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="0f566-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f566-129">Property</span></span>|<span data-ttu-id="0f566-130">型</span><span class="sxs-lookup"><span data-stu-id="0f566-130">Type</span></span>|<span data-ttu-id="0f566-131">説明</span><span class="sxs-lookup"><span data-stu-id="0f566-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f566-132">id</span><span class="sxs-lookup"><span data-stu-id="0f566-132">id</span></span>|<span data-ttu-id="0f566-133">String</span><span class="sxs-lookup"><span data-stu-id="0f566-133">String</span></span>|<span data-ttu-id="0f566-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f566-134">Key of the entity.</span></span> <span data-ttu-id="0f566-135">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0f566-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="0f566-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="0f566-136">appUserModelId</span></span>|<span data-ttu-id="0f566-137">文字列</span><span class="sxs-lookup"><span data-stu-id="0f566-137">String</span></span>|<span data-ttu-id="0f566-138">WindowsUniversalAppX アプリの含まれているアプリのアプリユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="0f566-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="0f566-139">応答</span><span class="sxs-lookup"><span data-stu-id="0f566-139">Response</span></span>
<span data-ttu-id="0f566-140">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f566-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f566-141">例</span><span class="sxs-lookup"><span data-stu-id="0f566-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f566-142">要求</span><span class="sxs-lookup"><span data-stu-id="0f566-142">Request</span></span>
<span data-ttu-id="0f566-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f566-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="0f566-144">応答</span><span class="sxs-lookup"><span data-stu-id="0f566-144">Response</span></span>
<span data-ttu-id="0f566-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f566-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```





