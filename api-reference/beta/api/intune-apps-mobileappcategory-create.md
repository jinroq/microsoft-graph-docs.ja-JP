---
title: mobileAppCategory の作成
description: 新しい mobileAppCategory オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e88632627569af8a77ff60b11b7319b2acdaf430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423861"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="a577c-103">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="a577c-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="a577c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a577c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a577c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a577c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a577c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a577c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a577c-107">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a577c-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a577c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a577c-108">Prerequisites</span></span>
<span data-ttu-id="a577c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a577c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a577c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a577c-111">Permission type</span></span>|<span data-ttu-id="a577c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a577c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a577c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a577c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a577c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a577c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a577c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a577c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a577c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a577c-116">Not supported.</span></span>|
|<span data-ttu-id="a577c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a577c-117">Application</span></span>|<span data-ttu-id="a577c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a577c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a577c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a577c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="a577c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a577c-120">Request headers</span></span>
|<span data-ttu-id="a577c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a577c-121">Header</span></span>|<span data-ttu-id="a577c-122">値</span><span class="sxs-lookup"><span data-stu-id="a577c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a577c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a577c-123">Authorization</span></span>|<span data-ttu-id="a577c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a577c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a577c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a577c-125">Accept</span></span>|<span data-ttu-id="a577c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a577c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a577c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a577c-127">Request body</span></span>
<span data-ttu-id="a577c-128">要求本文で、mobileAppCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a577c-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="a577c-129">次の表に、mobileAppCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a577c-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="a577c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a577c-130">Property</span></span>|<span data-ttu-id="a577c-131">型</span><span class="sxs-lookup"><span data-stu-id="a577c-131">Type</span></span>|<span data-ttu-id="a577c-132">説明</span><span class="sxs-lookup"><span data-stu-id="a577c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a577c-133">id</span><span class="sxs-lookup"><span data-stu-id="a577c-133">id</span></span>|<span data-ttu-id="a577c-134">String</span><span class="sxs-lookup"><span data-stu-id="a577c-134">String</span></span>|<span data-ttu-id="a577c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a577c-135">The key of the entity.</span></span>|
|<span data-ttu-id="a577c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a577c-136">displayName</span></span>|<span data-ttu-id="a577c-137">String</span><span class="sxs-lookup"><span data-stu-id="a577c-137">String</span></span>|<span data-ttu-id="a577c-138">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="a577c-138">The name of the app category.</span></span>|
|<span data-ttu-id="a577c-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a577c-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a577c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a577c-140">DateTimeOffset</span></span>|<span data-ttu-id="a577c-141">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a577c-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a577c-142">応答</span><span class="sxs-lookup"><span data-stu-id="a577c-142">Response</span></span>
<span data-ttu-id="a577c-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a577c-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a577c-144">例</span><span class="sxs-lookup"><span data-stu-id="a577c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a577c-145">要求</span><span class="sxs-lookup"><span data-stu-id="a577c-145">Request</span></span>
<span data-ttu-id="a577c-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a577c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a577c-147">応答</span><span class="sxs-lookup"><span data-stu-id="a577c-147">Response</span></span>
<span data-ttu-id="a577c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a577c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




