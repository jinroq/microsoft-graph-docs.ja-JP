---
title: mobileAppCategory の作成
description: 新しい mobileAppCategory オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aaf8fb298488b6de09fb875a9a87ab676a0c9cd3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935280"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="8598d-103">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="8598d-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="8598d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8598d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8598d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8598d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8598d-106">新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8598d-106">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8598d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8598d-107">Prerequisites</span></span>
<span data-ttu-id="8598d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8598d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8598d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8598d-110">Permission type</span></span>|<span data-ttu-id="8598d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8598d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8598d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8598d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8598d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8598d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8598d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8598d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8598d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8598d-115">Not supported.</span></span>|
|<span data-ttu-id="8598d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8598d-116">Application</span></span>|<span data-ttu-id="8598d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8598d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8598d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8598d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="8598d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8598d-119">Request headers</span></span>
|<span data-ttu-id="8598d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8598d-120">Header</span></span>|<span data-ttu-id="8598d-121">値</span><span class="sxs-lookup"><span data-stu-id="8598d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8598d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8598d-122">Authorization</span></span>|<span data-ttu-id="8598d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8598d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8598d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8598d-124">Accept</span></span>|<span data-ttu-id="8598d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8598d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8598d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8598d-126">Request body</span></span>
<span data-ttu-id="8598d-127">要求本文で、mobileAppCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8598d-127">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="8598d-128">次の表に、mobileAppCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8598d-128">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="8598d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8598d-129">Property</span></span>|<span data-ttu-id="8598d-130">型</span><span class="sxs-lookup"><span data-stu-id="8598d-130">Type</span></span>|<span data-ttu-id="8598d-131">説明</span><span class="sxs-lookup"><span data-stu-id="8598d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8598d-132">id</span><span class="sxs-lookup"><span data-stu-id="8598d-132">id</span></span>|<span data-ttu-id="8598d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8598d-133">String</span></span>|<span data-ttu-id="8598d-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8598d-134">The key of the entity.</span></span>|
|<span data-ttu-id="8598d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8598d-135">displayName</span></span>|<span data-ttu-id="8598d-136">String</span><span class="sxs-lookup"><span data-stu-id="8598d-136">String</span></span>|<span data-ttu-id="8598d-137">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="8598d-137">The name of the app category.</span></span>|
|<span data-ttu-id="8598d-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8598d-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8598d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8598d-139">DateTimeOffset</span></span>|<span data-ttu-id="8598d-140">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8598d-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8598d-141">応答</span><span class="sxs-lookup"><span data-stu-id="8598d-141">Response</span></span>
<span data-ttu-id="8598d-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8598d-142">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8598d-143">例</span><span class="sxs-lookup"><span data-stu-id="8598d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8598d-144">要求</span><span class="sxs-lookup"><span data-stu-id="8598d-144">Request</span></span>
<span data-ttu-id="8598d-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8598d-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="8598d-146">応答</span><span class="sxs-lookup"><span data-stu-id="8598d-146">Response</span></span>
<span data-ttu-id="8598d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8598d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




