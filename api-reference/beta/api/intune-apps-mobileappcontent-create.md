---
title: mobileAppContent の作成
description: 新しい mobileAppContent オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82a8e0fdd96235f319685dec5223a358421ea8f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404744"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="e93f7-103">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="e93f7-103">Create mobileAppContent</span></span>

> <span data-ttu-id="e93f7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e93f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e93f7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e93f7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e93f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e93f7-107">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e93f7-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e93f7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e93f7-108">Prerequisites</span></span>
<span data-ttu-id="e93f7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e93f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e93f7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e93f7-111">Permission type</span></span>|<span data-ttu-id="e93f7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e93f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e93f7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e93f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e93f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e93f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e93f7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e93f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e93f7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93f7-116">Not supported.</span></span>|
|<span data-ttu-id="e93f7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e93f7-117">Application</span></span>|<span data-ttu-id="e93f7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e93f7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e93f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="e93f7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e93f7-120">Request headers</span></span>
|<span data-ttu-id="e93f7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e93f7-121">Header</span></span>|<span data-ttu-id="e93f7-122">値</span><span class="sxs-lookup"><span data-stu-id="e93f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e93f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e93f7-123">Authorization</span></span>|<span data-ttu-id="e93f7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e93f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e93f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e93f7-125">Accept</span></span>|<span data-ttu-id="e93f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e93f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e93f7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e93f7-127">Request body</span></span>
<span data-ttu-id="e93f7-128">要求本文で、mobileAppContent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e93f7-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="e93f7-129">次の表に、mobileAppContent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e93f7-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="e93f7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e93f7-130">Property</span></span>|<span data-ttu-id="e93f7-131">型</span><span class="sxs-lookup"><span data-stu-id="e93f7-131">Type</span></span>|<span data-ttu-id="e93f7-132">説明</span><span class="sxs-lookup"><span data-stu-id="e93f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e93f7-133">id</span><span class="sxs-lookup"><span data-stu-id="e93f7-133">id</span></span>|<span data-ttu-id="e93f7-134">String</span><span class="sxs-lookup"><span data-stu-id="e93f7-134">String</span></span>|<span data-ttu-id="e93f7-135">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e93f7-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="e93f7-136">応答</span><span class="sxs-lookup"><span data-stu-id="e93f7-136">Response</span></span>
<span data-ttu-id="e93f7-137">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e93f7-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e93f7-138">例</span><span class="sxs-lookup"><span data-stu-id="e93f7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e93f7-139">要求</span><span class="sxs-lookup"><span data-stu-id="e93f7-139">Request</span></span>
<span data-ttu-id="e93f7-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e93f7-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="e93f7-141">応答</span><span class="sxs-lookup"><span data-stu-id="e93f7-141">Response</span></span>
<span data-ttu-id="e93f7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e93f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




