---
title: DeviceManagementTemplateSettingCategory の更新
description: DeviceManagementTemplateSettingCategory オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7df91d50f04ab5fc0053f0809ea381d0541366da
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313070"
---
# <a name="update-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="afa38-103">DeviceManagementTemplateSettingCategory の更新</span><span class="sxs-lookup"><span data-stu-id="afa38-103">Update deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="afa38-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afa38-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="afa38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afa38-106">[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="afa38-106">Update the properties of a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afa38-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="afa38-107">Prerequisites</span></span>
<span data-ttu-id="afa38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afa38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa38-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afa38-110">Permission type</span></span>|<span data-ttu-id="afa38-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="afa38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afa38-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afa38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afa38-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa38-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afa38-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afa38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afa38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa38-115">Not supported.</span></span>|
|<span data-ttu-id="afa38-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afa38-116">Application</span></span>|<span data-ttu-id="afa38-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa38-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afa38-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afa38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="afa38-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afa38-119">Request headers</span></span>
|<span data-ttu-id="afa38-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afa38-120">Header</span></span>|<span data-ttu-id="afa38-121">値</span><span class="sxs-lookup"><span data-stu-id="afa38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afa38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afa38-122">Authorization</span></span>|<span data-ttu-id="afa38-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="afa38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afa38-124">承諾</span><span class="sxs-lookup"><span data-stu-id="afa38-124">Accept</span></span>|<span data-ttu-id="afa38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afa38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afa38-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="afa38-126">Request body</span></span>
<span data-ttu-id="afa38-127">要求本文で、 [Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="afa38-127">In the request body, supply a JSON representation for the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

<span data-ttu-id="afa38-128">次の表に、 [Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="afa38-128">The following table shows the properties that are required when you create the [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).</span></span>

|<span data-ttu-id="afa38-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afa38-129">Property</span></span>|<span data-ttu-id="afa38-130">型</span><span class="sxs-lookup"><span data-stu-id="afa38-130">Type</span></span>|<span data-ttu-id="afa38-131">説明</span><span class="sxs-lookup"><span data-stu-id="afa38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afa38-132">id</span><span class="sxs-lookup"><span data-stu-id="afa38-132">id</span></span>|<span data-ttu-id="afa38-133">文字列</span><span class="sxs-lookup"><span data-stu-id="afa38-133">String</span></span>|<span data-ttu-id="afa38-134">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="afa38-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="afa38-135">displayName</span><span class="sxs-lookup"><span data-stu-id="afa38-135">displayName</span></span>|<span data-ttu-id="afa38-136">String</span><span class="sxs-lookup"><span data-stu-id="afa38-136">String</span></span>|<span data-ttu-id="afa38-137">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名</span><span class="sxs-lookup"><span data-stu-id="afa38-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="afa38-138">応答</span><span class="sxs-lookup"><span data-stu-id="afa38-138">Response</span></span>
<span data-ttu-id="afa38-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="afa38-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afa38-140">例</span><span class="sxs-lookup"><span data-stu-id="afa38-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="afa38-141">要求</span><span class="sxs-lookup"><span data-stu-id="afa38-141">Request</span></span>
<span data-ttu-id="afa38-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afa38-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="afa38-143">応答</span><span class="sxs-lookup"><span data-stu-id="afa38-143">Response</span></span>
<span data-ttu-id="afa38-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afa38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 170

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value"
}
```






