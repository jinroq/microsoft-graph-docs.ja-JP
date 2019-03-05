---
title: mobileAppCategory の作成
description: 新しい mobileAppCategory オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d540c906bbf0f2b096f2a9d2fb1fa65101fba10
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253849"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="b4642-103">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="b4642-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="b4642-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4642-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4642-105">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4642-105">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4642-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4642-106">Prerequisites</span></span>
<span data-ttu-id="b4642-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4642-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4642-109">Permission type</span></span>|<span data-ttu-id="b4642-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4642-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4642-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4642-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4642-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4642-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4642-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4642-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4642-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4642-114">Not supported.</span></span>|
|<span data-ttu-id="b4642-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4642-115">Application</span></span>|<span data-ttu-id="b4642-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4642-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4642-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4642-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="b4642-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4642-118">Request headers</span></span>
|<span data-ttu-id="b4642-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4642-119">Header</span></span>|<span data-ttu-id="b4642-120">値</span><span class="sxs-lookup"><span data-stu-id="b4642-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4642-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4642-121">Authorization</span></span>|<span data-ttu-id="b4642-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b4642-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4642-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b4642-123">Accept</span></span>|<span data-ttu-id="b4642-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4642-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4642-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4642-125">Request body</span></span>
<span data-ttu-id="b4642-126">要求本文で、mobileAppCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b4642-126">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="b4642-127">次の表に、mobileAppCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b4642-127">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="b4642-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4642-128">Property</span></span>|<span data-ttu-id="b4642-129">型</span><span class="sxs-lookup"><span data-stu-id="b4642-129">Type</span></span>|<span data-ttu-id="b4642-130">説明</span><span class="sxs-lookup"><span data-stu-id="b4642-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4642-131">id</span><span class="sxs-lookup"><span data-stu-id="b4642-131">id</span></span>|<span data-ttu-id="b4642-132">String</span><span class="sxs-lookup"><span data-stu-id="b4642-132">String</span></span>|<span data-ttu-id="b4642-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b4642-133">The key of the entity.</span></span>|
|<span data-ttu-id="b4642-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b4642-134">displayName</span></span>|<span data-ttu-id="b4642-135">String</span><span class="sxs-lookup"><span data-stu-id="b4642-135">String</span></span>|<span data-ttu-id="b4642-136">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="b4642-136">The name of the app category.</span></span>|
|<span data-ttu-id="b4642-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4642-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b4642-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4642-138">DateTimeOffset</span></span>|<span data-ttu-id="b4642-139">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b4642-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b4642-140">応答</span><span class="sxs-lookup"><span data-stu-id="b4642-140">Response</span></span>
<span data-ttu-id="b4642-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b4642-141">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4642-142">例</span><span class="sxs-lookup"><span data-stu-id="b4642-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4642-143">要求</span><span class="sxs-lookup"><span data-stu-id="b4642-143">Request</span></span>
<span data-ttu-id="b4642-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4642-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="b4642-145">応答</span><span class="sxs-lookup"><span data-stu-id="b4642-145">Response</span></span>
<span data-ttu-id="b4642-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4642-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



