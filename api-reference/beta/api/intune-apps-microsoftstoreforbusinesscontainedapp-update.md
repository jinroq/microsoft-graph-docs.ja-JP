---
title: MicrosoftStoreForBusinessContainedApp の更新
description: MicrosoftStoreForBusinessContainedApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1dd8b87f550556833fe00c6ed2235687b098ffef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329398"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="ab21f-103">MicrosoftStoreForBusinessContainedApp の更新</span><span class="sxs-lookup"><span data-stu-id="ab21f-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="ab21f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab21f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab21f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab21f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab21f-106">[MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab21f-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab21f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ab21f-107">Prerequisites</span></span>
<span data-ttu-id="ab21f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab21f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab21f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab21f-110">Permission type</span></span>|<span data-ttu-id="ab21f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab21f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab21f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab21f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab21f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab21f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab21f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab21f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab21f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab21f-115">Not supported.</span></span>|
|<span data-ttu-id="ab21f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab21f-116">Application</span></span>|<span data-ttu-id="ab21f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab21f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab21f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab21f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ab21f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab21f-119">Request headers</span></span>
|<span data-ttu-id="ab21f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab21f-120">Header</span></span>|<span data-ttu-id="ab21f-121">値</span><span class="sxs-lookup"><span data-stu-id="ab21f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab21f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab21f-122">Authorization</span></span>|<span data-ttu-id="ab21f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab21f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab21f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ab21f-124">Accept</span></span>|<span data-ttu-id="ab21f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab21f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab21f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab21f-126">Request body</span></span>
<span data-ttu-id="ab21f-127">要求本文で、 [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab21f-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="ab21f-128">次の表に、 [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ab21f-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="ab21f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab21f-129">Property</span></span>|<span data-ttu-id="ab21f-130">型</span><span class="sxs-lookup"><span data-stu-id="ab21f-130">Type</span></span>|<span data-ttu-id="ab21f-131">説明</span><span class="sxs-lookup"><span data-stu-id="ab21f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab21f-132">id</span><span class="sxs-lookup"><span data-stu-id="ab21f-132">id</span></span>|<span data-ttu-id="ab21f-133">String</span><span class="sxs-lookup"><span data-stu-id="ab21f-133">String</span></span>|<span data-ttu-id="ab21f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ab21f-134">Key of the entity.</span></span> <span data-ttu-id="ab21f-135">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ab21f-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="ab21f-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="ab21f-136">appUserModelId</span></span>|<span data-ttu-id="ab21f-137">String</span><span class="sxs-lookup"><span data-stu-id="ab21f-137">String</span></span>|<span data-ttu-id="ab21f-138">Microsoft Storeforbusinessapp の含まれているアプリのアプリケーションユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="ab21f-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="ab21f-139">応答</span><span class="sxs-lookup"><span data-stu-id="ab21f-139">Response</span></span>
<span data-ttu-id="ab21f-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab21f-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab21f-141">例</span><span class="sxs-lookup"><span data-stu-id="ab21f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab21f-142">要求</span><span class="sxs-lookup"><span data-stu-id="ab21f-142">Request</span></span>
<span data-ttu-id="ab21f-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab21f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="ab21f-144">応答</span><span class="sxs-lookup"><span data-stu-id="ab21f-144">Response</span></span>
<span data-ttu-id="ab21f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab21f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```






