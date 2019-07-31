---
title: MicrosoftStoreForBusinessContainedApp を作成する
description: 新しい microsoftStoreForBusinessContainedApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34b154323a52f873eae2e50aab65d7419ab2abf8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961176"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="4a102-103">MicrosoftStoreForBusinessContainedApp を作成する</span><span class="sxs-lookup"><span data-stu-id="4a102-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="4a102-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a102-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a102-106">新しい[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a102-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a102-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4a102-107">Prerequisites</span></span>
<span data-ttu-id="4a102-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a102-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a102-110">Permission type</span></span>|<span data-ttu-id="4a102-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a102-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a102-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a102-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a102-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a102-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a102-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a102-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a102-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a102-115">Not supported.</span></span>|
|<span data-ttu-id="4a102-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a102-116">Application</span></span>|<span data-ttu-id="4a102-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a102-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a102-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a102-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="4a102-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a102-119">Request headers</span></span>
|<span data-ttu-id="4a102-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a102-120">Header</span></span>|<span data-ttu-id="4a102-121">値</span><span class="sxs-lookup"><span data-stu-id="4a102-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a102-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a102-122">Authorization</span></span>|<span data-ttu-id="4a102-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a102-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a102-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4a102-124">Accept</span></span>|<span data-ttu-id="4a102-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a102-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a102-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a102-126">Request body</span></span>
<span data-ttu-id="4a102-127">要求本文で、microsoftStoreForBusinessContainedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a102-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="4a102-128">次の表に、microsoftStoreForBusinessContainedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4a102-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="4a102-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a102-129">Property</span></span>|<span data-ttu-id="4a102-130">型</span><span class="sxs-lookup"><span data-stu-id="4a102-130">Type</span></span>|<span data-ttu-id="4a102-131">説明</span><span class="sxs-lookup"><span data-stu-id="4a102-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a102-132">id</span><span class="sxs-lookup"><span data-stu-id="4a102-132">id</span></span>|<span data-ttu-id="4a102-133">String</span><span class="sxs-lookup"><span data-stu-id="4a102-133">String</span></span>|<span data-ttu-id="4a102-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4a102-134">Key of the entity.</span></span> <span data-ttu-id="4a102-135">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4a102-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="4a102-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="4a102-136">appUserModelId</span></span>|<span data-ttu-id="4a102-137">String</span><span class="sxs-lookup"><span data-stu-id="4a102-137">String</span></span>|<span data-ttu-id="4a102-138">Microsoft Storeforbusinessapp の含まれているアプリのアプリケーションユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="4a102-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="4a102-139">応答</span><span class="sxs-lookup"><span data-stu-id="4a102-139">Response</span></span>
<span data-ttu-id="4a102-140">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a102-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a102-141">例</span><span class="sxs-lookup"><span data-stu-id="4a102-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a102-142">要求</span><span class="sxs-lookup"><span data-stu-id="4a102-142">Request</span></span>
<span data-ttu-id="4a102-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a102-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="4a102-144">応答</span><span class="sxs-lookup"><span data-stu-id="4a102-144">Response</span></span>
<span data-ttu-id="4a102-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a102-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





