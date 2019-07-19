---
title: DeviceManagementScriptGroupAssignment の作成
description: 新しい deviceManagementScriptGroupAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e3079da0aadd24ef0b36d3e5a02c9c979380c37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958887"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="8ace7-103">DeviceManagementScriptGroupAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="8ace7-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="8ace7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ace7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ace7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ace7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ace7-106">新しい[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ace7-106">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ace7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ace7-107">Prerequisites</span></span>
<span data-ttu-id="8ace7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ace7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ace7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ace7-110">Permission type</span></span>|<span data-ttu-id="8ace7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ace7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ace7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ace7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ace7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ace7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ace7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ace7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ace7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ace7-115">Not supported.</span></span>|
|<span data-ttu-id="8ace7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ace7-116">Application</span></span>|<span data-ttu-id="8ace7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ace7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ace7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ace7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="8ace7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ace7-119">Request headers</span></span>
|<span data-ttu-id="8ace7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ace7-120">Header</span></span>|<span data-ttu-id="8ace7-121">値</span><span class="sxs-lookup"><span data-stu-id="8ace7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ace7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ace7-122">Authorization</span></span>|<span data-ttu-id="8ace7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ace7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ace7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8ace7-124">Accept</span></span>|<span data-ttu-id="8ace7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ace7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ace7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ace7-126">Request body</span></span>
<span data-ttu-id="8ace7-127">要求本文で、deviceManagementScriptGroupAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ace7-127">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="8ace7-128">次の表に、deviceManagementScriptGroupAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8ace7-128">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="8ace7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ace7-129">Property</span></span>|<span data-ttu-id="8ace7-130">型</span><span class="sxs-lookup"><span data-stu-id="8ace7-130">Type</span></span>|<span data-ttu-id="8ace7-131">説明</span><span class="sxs-lookup"><span data-stu-id="8ace7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ace7-132">id</span><span class="sxs-lookup"><span data-stu-id="8ace7-132">id</span></span>|<span data-ttu-id="8ace7-133">String</span><span class="sxs-lookup"><span data-stu-id="8ace7-133">String</span></span>|<span data-ttu-id="8ace7-134">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8ace7-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="8ace7-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="8ace7-135">targetGroupId</span></span>|<span data-ttu-id="8ace7-136">String</span><span class="sxs-lookup"><span data-stu-id="8ace7-136">String</span></span>|<span data-ttu-id="8ace7-137">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="8ace7-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="8ace7-138">応答</span><span class="sxs-lookup"><span data-stu-id="8ace7-138">Response</span></span>
<span data-ttu-id="8ace7-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ace7-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ace7-140">例</span><span class="sxs-lookup"><span data-stu-id="8ace7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ace7-141">要求</span><span class="sxs-lookup"><span data-stu-id="8ace7-141">Request</span></span>
<span data-ttu-id="8ace7-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ace7-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="8ace7-143">応答</span><span class="sxs-lookup"><span data-stu-id="8ace7-143">Response</span></span>
<span data-ttu-id="8ace7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ace7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





