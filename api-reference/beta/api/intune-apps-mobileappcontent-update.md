---
title: mobileAppContent の更新
description: mobileAppContent オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 262a7fc48e30e816b07aae963a0951ed4605925d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413375"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="b4f05-103">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="b4f05-103">Update mobileAppContent</span></span>

> <span data-ttu-id="b4f05-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4f05-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4f05-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4f05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4f05-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4f05-107">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b4f05-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4f05-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4f05-108">Prerequisites</span></span>
<span data-ttu-id="b4f05-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4f05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4f05-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4f05-111">Permission type</span></span>|<span data-ttu-id="b4f05-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4f05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4f05-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4f05-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f05-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4f05-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4f05-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4f05-116">Not supported.</span></span>|
|<span data-ttu-id="b4f05-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4f05-117">Application</span></span>|<span data-ttu-id="b4f05-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4f05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4f05-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="b4f05-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4f05-120">Request headers</span></span>
|<span data-ttu-id="b4f05-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4f05-121">Header</span></span>|<span data-ttu-id="b4f05-122">値</span><span class="sxs-lookup"><span data-stu-id="b4f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4f05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4f05-123">Authorization</span></span>|<span data-ttu-id="b4f05-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b4f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4f05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4f05-125">Accept</span></span>|<span data-ttu-id="b4f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4f05-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4f05-127">Request body</span></span>
<span data-ttu-id="b4f05-128">要求本文で、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b4f05-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="b4f05-129">次の表に、[mobileAppContent](../resources/intune-apps-mobileappcontent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b4f05-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="b4f05-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4f05-130">Property</span></span>|<span data-ttu-id="b4f05-131">型</span><span class="sxs-lookup"><span data-stu-id="b4f05-131">Type</span></span>|<span data-ttu-id="b4f05-132">説明</span><span class="sxs-lookup"><span data-stu-id="b4f05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4f05-133">id</span><span class="sxs-lookup"><span data-stu-id="b4f05-133">id</span></span>|<span data-ttu-id="b4f05-134">String</span><span class="sxs-lookup"><span data-stu-id="b4f05-134">String</span></span>|<span data-ttu-id="b4f05-135">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b4f05-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="b4f05-136">応答</span><span class="sxs-lookup"><span data-stu-id="b4f05-136">Response</span></span>
<span data-ttu-id="b4f05-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b4f05-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4f05-138">例</span><span class="sxs-lookup"><span data-stu-id="b4f05-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4f05-139">要求</span><span class="sxs-lookup"><span data-stu-id="b4f05-139">Request</span></span>
<span data-ttu-id="b4f05-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4f05-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="b4f05-141">応答</span><span class="sxs-lookup"><span data-stu-id="b4f05-141">Response</span></span>
<span data-ttu-id="b4f05-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4f05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




