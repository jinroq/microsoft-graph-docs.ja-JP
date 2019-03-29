---
title: mobileAppCategory の更新
description: mobileAppCategory オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17f3a0c8a71e7c443764d03ba7021ecddfd5d7af
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979012"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="4d7ef-103">mobileAppCategory の更新</span><span class="sxs-lookup"><span data-stu-id="4d7ef-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="4d7ef-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d7ef-105">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d7ef-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4d7ef-106">Prerequisites</span></span>
<span data-ttu-id="4d7ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d7ef-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d7ef-109">Permission type</span></span>|<span data-ttu-id="4d7ef-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d7ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d7ef-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d7ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d7ef-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7ef-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d7ef-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d7ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d7ef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-114">Not supported.</span></span>|
|<span data-ttu-id="4d7ef-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d7ef-115">Application</span></span>|<span data-ttu-id="4d7ef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d7ef-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d7ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4d7ef-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d7ef-118">Request headers</span></span>
|<span data-ttu-id="4d7ef-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d7ef-119">Header</span></span>|<span data-ttu-id="4d7ef-120">値</span><span class="sxs-lookup"><span data-stu-id="4d7ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d7ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d7ef-121">Authorization</span></span>|<span data-ttu-id="4d7ef-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d7ef-123">承諾</span><span class="sxs-lookup"><span data-stu-id="4d7ef-123">Accept</span></span>|<span data-ttu-id="4d7ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d7ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d7ef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d7ef-125">Request body</span></span>
<span data-ttu-id="4d7ef-126">要求本文で、[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="4d7ef-127">次の表に、[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="4d7ef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d7ef-128">Property</span></span>|<span data-ttu-id="4d7ef-129">型</span><span class="sxs-lookup"><span data-stu-id="4d7ef-129">Type</span></span>|<span data-ttu-id="4d7ef-130">説明</span><span class="sxs-lookup"><span data-stu-id="4d7ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d7ef-131">id</span><span class="sxs-lookup"><span data-stu-id="4d7ef-131">id</span></span>|<span data-ttu-id="4d7ef-132">String</span><span class="sxs-lookup"><span data-stu-id="4d7ef-132">String</span></span>|<span data-ttu-id="4d7ef-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-133">The key of the entity.</span></span>|
|<span data-ttu-id="4d7ef-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4d7ef-134">displayName</span></span>|<span data-ttu-id="4d7ef-135">String</span><span class="sxs-lookup"><span data-stu-id="4d7ef-135">String</span></span>|<span data-ttu-id="4d7ef-136">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-136">The name of the app category.</span></span>|
|<span data-ttu-id="4d7ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d7ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4d7ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d7ef-138">DateTimeOffset</span></span>|<span data-ttu-id="4d7ef-139">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4d7ef-140">応答</span><span class="sxs-lookup"><span data-stu-id="4d7ef-140">Response</span></span>
<span data-ttu-id="4d7ef-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d7ef-142">例</span><span class="sxs-lookup"><span data-stu-id="4d7ef-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d7ef-143">要求</span><span class="sxs-lookup"><span data-stu-id="4d7ef-143">Request</span></span>
<span data-ttu-id="4d7ef-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4d7ef-145">応答</span><span class="sxs-lookup"><span data-stu-id="4d7ef-145">Response</span></span>
<span data-ttu-id="4d7ef-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d7ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



