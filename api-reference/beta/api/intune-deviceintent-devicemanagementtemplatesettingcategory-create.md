---
title: DeviceManagementTemplateSettingCategory の作成
description: 新しい deviceManagementTemplateSettingCategory オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 368491eda8ed4e13d7600073e859ceed73d6b094
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959685"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="9b193-103">DeviceManagementTemplateSettingCategory の作成</span><span class="sxs-lookup"><span data-stu-id="9b193-103">Create deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="9b193-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b193-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b193-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b193-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b193-106">新しい[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b193-106">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b193-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b193-107">Prerequisites</span></span>
<span data-ttu-id="9b193-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b193-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b193-110">Permission type</span></span>|<span data-ttu-id="9b193-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b193-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b193-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b193-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b193-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b193-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b193-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b193-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b193-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b193-115">Not supported.</span></span>|
|<span data-ttu-id="9b193-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b193-116">Application</span></span>|<span data-ttu-id="9b193-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b193-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b193-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b193-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="9b193-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b193-119">Request headers</span></span>
|<span data-ttu-id="9b193-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b193-120">Header</span></span>|<span data-ttu-id="9b193-121">値</span><span class="sxs-lookup"><span data-stu-id="9b193-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b193-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b193-122">Authorization</span></span>|<span data-ttu-id="9b193-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b193-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b193-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9b193-124">Accept</span></span>|<span data-ttu-id="9b193-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b193-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b193-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b193-126">Request body</span></span>
<span data-ttu-id="9b193-127">要求本文で、deviceManagementTemplateSettingCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b193-127">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="9b193-128">次の表に、deviceManagementTemplateSettingCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9b193-128">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="9b193-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b193-129">Property</span></span>|<span data-ttu-id="9b193-130">型</span><span class="sxs-lookup"><span data-stu-id="9b193-130">Type</span></span>|<span data-ttu-id="9b193-131">説明</span><span class="sxs-lookup"><span data-stu-id="9b193-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b193-132">id</span><span class="sxs-lookup"><span data-stu-id="9b193-132">id</span></span>|<span data-ttu-id="9b193-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9b193-133">String</span></span>|<span data-ttu-id="9b193-134">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="9b193-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="9b193-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9b193-135">displayName</span></span>|<span data-ttu-id="9b193-136">String</span><span class="sxs-lookup"><span data-stu-id="9b193-136">String</span></span>|<span data-ttu-id="9b193-137">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名</span><span class="sxs-lookup"><span data-stu-id="9b193-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9b193-138">応答</span><span class="sxs-lookup"><span data-stu-id="9b193-138">Response</span></span>
<span data-ttu-id="9b193-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b193-139">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b193-140">例</span><span class="sxs-lookup"><span data-stu-id="9b193-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b193-141">要求</span><span class="sxs-lookup"><span data-stu-id="9b193-141">Request</span></span>
<span data-ttu-id="9b193-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b193-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="9b193-143">応答</span><span class="sxs-lookup"><span data-stu-id="9b193-143">Response</span></span>
<span data-ttu-id="9b193-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b193-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 170

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value"
}
```





