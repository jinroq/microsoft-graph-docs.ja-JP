---
title: mobileAppContent の作成
description: 新しい mobileAppContent オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8660ffcb37bcf900f257a052f420aec26985e767
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960896"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="2ac68-103">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="2ac68-103">Create mobileAppContent</span></span>

> <span data-ttu-id="2ac68-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ac68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac68-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ac68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac68-106">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2ac68-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ac68-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ac68-107">Prerequisites</span></span>
<span data-ttu-id="2ac68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ac68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ac68-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ac68-110">Permission type</span></span>|<span data-ttu-id="2ac68-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ac68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac68-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ac68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ac68-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac68-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ac68-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ac68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac68-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ac68-115">Not supported.</span></span>|
|<span data-ttu-id="2ac68-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ac68-116">Application</span></span>|<span data-ttu-id="2ac68-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ac68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac68-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ac68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="2ac68-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ac68-119">Request headers</span></span>
|<span data-ttu-id="2ac68-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ac68-120">Header</span></span>|<span data-ttu-id="2ac68-121">値</span><span class="sxs-lookup"><span data-stu-id="2ac68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ac68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ac68-122">Authorization</span></span>|<span data-ttu-id="2ac68-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ac68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ac68-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2ac68-124">Accept</span></span>|<span data-ttu-id="2ac68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ac68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac68-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ac68-126">Request body</span></span>
<span data-ttu-id="2ac68-127">要求本文で、mobileAppContent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ac68-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="2ac68-128">次の表に、mobileAppContent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2ac68-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="2ac68-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ac68-129">Property</span></span>|<span data-ttu-id="2ac68-130">型</span><span class="sxs-lookup"><span data-stu-id="2ac68-130">Type</span></span>|<span data-ttu-id="2ac68-131">説明</span><span class="sxs-lookup"><span data-stu-id="2ac68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac68-132">id</span><span class="sxs-lookup"><span data-stu-id="2ac68-132">id</span></span>|<span data-ttu-id="2ac68-133">String</span><span class="sxs-lookup"><span data-stu-id="2ac68-133">String</span></span>|<span data-ttu-id="2ac68-134">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ac68-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="2ac68-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ac68-135">Response</span></span>
<span data-ttu-id="2ac68-136">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ac68-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ac68-137">例</span><span class="sxs-lookup"><span data-stu-id="2ac68-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ac68-138">要求</span><span class="sxs-lookup"><span data-stu-id="2ac68-138">Request</span></span>
<span data-ttu-id="2ac68-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ac68-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="2ac68-140">応答</span><span class="sxs-lookup"><span data-stu-id="2ac68-140">Response</span></span>
<span data-ttu-id="2ac68-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ac68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





