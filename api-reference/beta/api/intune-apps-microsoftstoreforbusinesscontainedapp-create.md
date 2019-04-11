---
title: microsoftStoreForBusinessContainedApp を作成する
description: 新しい microsoftStoreForBusinessContainedApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7d8894e01b7993e50f12ee3aa3e83173fbebb11
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795675"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="f25ba-103">microsoftStoreForBusinessContainedApp を作成する</span><span class="sxs-lookup"><span data-stu-id="f25ba-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="f25ba-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f25ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f25ba-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f25ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f25ba-106">新しい[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f25ba-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f25ba-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f25ba-107">Prerequisites</span></span>
<span data-ttu-id="f25ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f25ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f25ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f25ba-110">Permission type</span></span>|<span data-ttu-id="f25ba-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f25ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f25ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f25ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f25ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f25ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f25ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f25ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f25ba-115">Not supported.</span></span>|
|<span data-ttu-id="f25ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f25ba-116">Application</span></span>|<span data-ttu-id="f25ba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f25ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f25ba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f25ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="f25ba-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f25ba-119">Request headers</span></span>
|<span data-ttu-id="f25ba-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f25ba-120">Header</span></span>|<span data-ttu-id="f25ba-121">値</span><span class="sxs-lookup"><span data-stu-id="f25ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f25ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f25ba-122">Authorization</span></span>|<span data-ttu-id="f25ba-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f25ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f25ba-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f25ba-124">Accept</span></span>|<span data-ttu-id="f25ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f25ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f25ba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f25ba-126">Request body</span></span>
<span data-ttu-id="f25ba-127">要求本文で、microsoftStoreForBusinessContainedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f25ba-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="f25ba-128">次の表に、microsoftStoreForBusinessContainedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f25ba-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="f25ba-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f25ba-129">Property</span></span>|<span data-ttu-id="f25ba-130">型</span><span class="sxs-lookup"><span data-stu-id="f25ba-130">Type</span></span>|<span data-ttu-id="f25ba-131">説明</span><span class="sxs-lookup"><span data-stu-id="f25ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f25ba-132">id</span><span class="sxs-lookup"><span data-stu-id="f25ba-132">id</span></span>|<span data-ttu-id="f25ba-133">String</span><span class="sxs-lookup"><span data-stu-id="f25ba-133">String</span></span>|<span data-ttu-id="f25ba-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f25ba-134">Key of the entity.</span></span> <span data-ttu-id="f25ba-135">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f25ba-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="f25ba-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="f25ba-136">appUserModelId</span></span>|<span data-ttu-id="f25ba-137">文字列</span><span class="sxs-lookup"><span data-stu-id="f25ba-137">String</span></span>|<span data-ttu-id="f25ba-138">microsoft storeforbusinessapp の含まれているアプリのアプリケーションユーザーモデル ID。</span><span class="sxs-lookup"><span data-stu-id="f25ba-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="f25ba-139">応答</span><span class="sxs-lookup"><span data-stu-id="f25ba-139">Response</span></span>
<span data-ttu-id="f25ba-140">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f25ba-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f25ba-141">例</span><span class="sxs-lookup"><span data-stu-id="f25ba-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f25ba-142">要求</span><span class="sxs-lookup"><span data-stu-id="f25ba-142">Request</span></span>
<span data-ttu-id="f25ba-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f25ba-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="f25ba-144">応答</span><span class="sxs-lookup"><span data-stu-id="f25ba-144">Response</span></span>
<span data-ttu-id="f25ba-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f25ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





