---
title: mobileAppContent の更新
description: mobileAppContent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2718dd551a1d9bf1d5210d3d668e0bd26951c6fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002028"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="044cc-103">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="044cc-103">Update mobileAppContent</span></span>

> <span data-ttu-id="044cc-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="044cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="044cc-105">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="044cc-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="044cc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="044cc-106">Prerequisites</span></span>
<span data-ttu-id="044cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="044cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="044cc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="044cc-109">Permission type</span></span>|<span data-ttu-id="044cc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="044cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="044cc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="044cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="044cc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044cc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="044cc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="044cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="044cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="044cc-114">Not supported.</span></span>|
|<span data-ttu-id="044cc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="044cc-115">Application</span></span>|<span data-ttu-id="044cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="044cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="044cc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="044cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="044cc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="044cc-118">Request headers</span></span>
|<span data-ttu-id="044cc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="044cc-119">Header</span></span>|<span data-ttu-id="044cc-120">値</span><span class="sxs-lookup"><span data-stu-id="044cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="044cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="044cc-121">Authorization</span></span>|<span data-ttu-id="044cc-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="044cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="044cc-123">承諾</span><span class="sxs-lookup"><span data-stu-id="044cc-123">Accept</span></span>|<span data-ttu-id="044cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="044cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="044cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="044cc-125">Request body</span></span>
<span data-ttu-id="044cc-126">要求本文で、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="044cc-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="044cc-127">次の表に、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="044cc-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="044cc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="044cc-128">Property</span></span>|<span data-ttu-id="044cc-129">型</span><span class="sxs-lookup"><span data-stu-id="044cc-129">Type</span></span>|<span data-ttu-id="044cc-130">説明</span><span class="sxs-lookup"><span data-stu-id="044cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="044cc-131">id</span><span class="sxs-lookup"><span data-stu-id="044cc-131">id</span></span>|<span data-ttu-id="044cc-132">String</span><span class="sxs-lookup"><span data-stu-id="044cc-132">String</span></span>|<span data-ttu-id="044cc-133">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="044cc-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="044cc-134">応答</span><span class="sxs-lookup"><span data-stu-id="044cc-134">Response</span></span>
<span data-ttu-id="044cc-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="044cc-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="044cc-136">例</span><span class="sxs-lookup"><span data-stu-id="044cc-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="044cc-137">要求</span><span class="sxs-lookup"><span data-stu-id="044cc-137">Request</span></span>
<span data-ttu-id="044cc-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="044cc-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="044cc-139">応答</span><span class="sxs-lookup"><span data-stu-id="044cc-139">Response</span></span>
<span data-ttu-id="044cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="044cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



