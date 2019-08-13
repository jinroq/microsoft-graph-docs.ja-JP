---
title: DeviceManagementIntentSettingCategory の作成
description: 新しい deviceManagementIntentSettingCategory オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 782361aed36923d8f49af25daa12b8f05ba24a18
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343518"
---
# <a name="create-devicemanagementintentsettingcategory"></a><span data-ttu-id="2af80-103">DeviceManagementIntentSettingCategory の作成</span><span class="sxs-lookup"><span data-stu-id="2af80-103">Create deviceManagementIntentSettingCategory</span></span>

> <span data-ttu-id="2af80-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2af80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2af80-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2af80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2af80-106">新しい[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2af80-106">Create a new [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2af80-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2af80-107">Prerequisites</span></span>
<span data-ttu-id="2af80-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2af80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2af80-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2af80-110">Permission type</span></span>|<span data-ttu-id="2af80-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2af80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2af80-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2af80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2af80-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af80-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2af80-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2af80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2af80-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2af80-115">Not supported.</span></span>|
|<span data-ttu-id="2af80-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2af80-116">Application</span></span>|<span data-ttu-id="2af80-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af80-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2af80-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2af80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="2af80-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2af80-119">Request headers</span></span>
|<span data-ttu-id="2af80-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2af80-120">Header</span></span>|<span data-ttu-id="2af80-121">値</span><span class="sxs-lookup"><span data-stu-id="2af80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2af80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af80-122">Authorization</span></span>|<span data-ttu-id="2af80-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2af80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2af80-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2af80-124">Accept</span></span>|<span data-ttu-id="2af80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2af80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2af80-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2af80-126">Request body</span></span>
<span data-ttu-id="2af80-127">要求本文で、deviceManagementIntentSettingCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2af80-127">In the request body, supply a JSON representation for the deviceManagementIntentSettingCategory object.</span></span>

<span data-ttu-id="2af80-128">次の表に、deviceManagementIntentSettingCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2af80-128">The following table shows the properties that are required when you create the deviceManagementIntentSettingCategory.</span></span>

|<span data-ttu-id="2af80-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2af80-129">Property</span></span>|<span data-ttu-id="2af80-130">型</span><span class="sxs-lookup"><span data-stu-id="2af80-130">Type</span></span>|<span data-ttu-id="2af80-131">説明</span><span class="sxs-lookup"><span data-stu-id="2af80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af80-132">id</span><span class="sxs-lookup"><span data-stu-id="2af80-132">id</span></span>|<span data-ttu-id="2af80-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2af80-133">String</span></span>|<span data-ttu-id="2af80-134">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="2af80-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="2af80-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2af80-135">displayName</span></span>|<span data-ttu-id="2af80-136">String</span><span class="sxs-lookup"><span data-stu-id="2af80-136">String</span></span>|<span data-ttu-id="2af80-137">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名</span><span class="sxs-lookup"><span data-stu-id="2af80-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2af80-138">応答</span><span class="sxs-lookup"><span data-stu-id="2af80-138">Response</span></span>
<span data-ttu-id="2af80-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2af80-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af80-140">例</span><span class="sxs-lookup"><span data-stu-id="2af80-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2af80-141">要求</span><span class="sxs-lookup"><span data-stu-id="2af80-141">Request</span></span>
<span data-ttu-id="2af80-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2af80-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="2af80-143">応答</span><span class="sxs-lookup"><span data-stu-id="2af80-143">Response</span></span>
<span data-ttu-id="2af80-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2af80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "39bf2a82-2a82-39bf-822a-bf39822abf39",
  "displayName": "Display Name value"
}
```






