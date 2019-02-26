---
title: mobileAppContent の更新
description: mobileAppContent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b792deab5c10e8770666a707976afa330d03a4f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149372"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="5b358-103">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="5b358-103">Update mobileAppContent</span></span>

> <span data-ttu-id="5b358-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b358-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b358-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b358-106">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b358-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b358-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5b358-107">Prerequisites</span></span>
<span data-ttu-id="5b358-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b358-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b358-110">Permission type</span></span>|<span data-ttu-id="5b358-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b358-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b358-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b358-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b358-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b358-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b358-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b358-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b358-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b358-115">Not supported.</span></span>|
|<span data-ttu-id="5b358-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b358-116">Application</span></span>|<span data-ttu-id="5b358-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b358-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b358-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b358-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="5b358-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b358-119">Request headers</span></span>
|<span data-ttu-id="5b358-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b358-120">Header</span></span>|<span data-ttu-id="5b358-121">値</span><span class="sxs-lookup"><span data-stu-id="5b358-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b358-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b358-122">Authorization</span></span>|<span data-ttu-id="5b358-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5b358-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b358-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5b358-124">Accept</span></span>|<span data-ttu-id="5b358-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b358-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b358-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b358-126">Request body</span></span>
<span data-ttu-id="5b358-127">要求本文で、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b358-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="5b358-128">次の表に、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5b358-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="5b358-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b358-129">Property</span></span>|<span data-ttu-id="5b358-130">型</span><span class="sxs-lookup"><span data-stu-id="5b358-130">Type</span></span>|<span data-ttu-id="5b358-131">説明</span><span class="sxs-lookup"><span data-stu-id="5b358-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b358-132">id</span><span class="sxs-lookup"><span data-stu-id="5b358-132">id</span></span>|<span data-ttu-id="5b358-133">String</span><span class="sxs-lookup"><span data-stu-id="5b358-133">String</span></span>|<span data-ttu-id="5b358-134">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5b358-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="5b358-135">応答</span><span class="sxs-lookup"><span data-stu-id="5b358-135">Response</span></span>
<span data-ttu-id="5b358-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b358-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b358-137">例</span><span class="sxs-lookup"><span data-stu-id="5b358-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b358-138">要求</span><span class="sxs-lookup"><span data-stu-id="5b358-138">Request</span></span>
<span data-ttu-id="5b358-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b358-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="5b358-140">応答</span><span class="sxs-lookup"><span data-stu-id="5b358-140">Response</span></span>
<span data-ttu-id="5b358-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b358-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




