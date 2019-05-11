---
title: DeviceConfigurationConflictSummary を作成する
description: 新しい deviceConfigurationConflictSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8bcc892e895babe22da90e1e9867cce96a195c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927366"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="ae1e6-103">DeviceConfigurationConflictSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="ae1e6-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="ae1e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae1e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1e6-106">新しい[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-106">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae1e6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae1e6-107">Prerequisites</span></span>
<span data-ttu-id="ae1e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae1e6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae1e6-110">Permission type</span></span>|<span data-ttu-id="ae1e6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae1e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae1e6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae1e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae1e6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae1e6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae1e6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae1e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae1e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-115">Not supported.</span></span>|
|<span data-ttu-id="ae1e6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae1e6-116">Application</span></span>|<span data-ttu-id="ae1e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae1e6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae1e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="ae1e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae1e6-119">Request headers</span></span>
|<span data-ttu-id="ae1e6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae1e6-120">Header</span></span>|<span data-ttu-id="ae1e6-121">値</span><span class="sxs-lookup"><span data-stu-id="ae1e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae1e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae1e6-122">Authorization</span></span>|<span data-ttu-id="ae1e6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae1e6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae1e6-124">Accept</span></span>|<span data-ttu-id="ae1e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae1e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae1e6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae1e6-126">Request body</span></span>
<span data-ttu-id="ae1e6-127">要求本文で、deviceConfigurationConflictSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-127">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="ae1e6-128">次の表に、deviceConfigurationConflictSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-128">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="ae1e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae1e6-129">Property</span></span>|<span data-ttu-id="ae1e6-130">型</span><span class="sxs-lookup"><span data-stu-id="ae1e6-130">Type</span></span>|<span data-ttu-id="ae1e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="ae1e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1e6-132">競合する Devicdeviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="ae1e6-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="ae1e6-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae1e6-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="ae1e6-134">指定された設定と競合しているポリシーのセット</span><span class="sxs-lookup"><span data-stu-id="ae1e6-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="ae1e6-135">id</span><span class="sxs-lookup"><span data-stu-id="ae1e6-135">id</span></span>|<span data-ttu-id="ae1e6-136">String</span><span class="sxs-lookup"><span data-stu-id="ae1e6-136">String</span></span>|<span data-ttu-id="ae1e6-137">競合しているポリシーのセットの id。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="ae1e6-138">この id は、アンダースコアで区切られた辞書順で競合しているすべてのポリシーの id です。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="ae1e6-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="ae1e6-139">contributingSettings</span></span>|<span data-ttu-id="ae1e6-140">String collection</span><span class="sxs-lookup"><span data-stu-id="ae1e6-140">String collection</span></span>|<span data-ttu-id="ae1e6-141">指定されたポリシーと競合する設定のセット</span><span class="sxs-lookup"><span data-stu-id="ae1e6-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="ae1e6-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="ae1e6-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="ae1e6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ae1e6-143">Int32</span></span>|<span data-ttu-id="ae1e6-144">競合するポリシーと設定によって影響を受けるチェックインの数</span><span class="sxs-lookup"><span data-stu-id="ae1e6-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="ae1e6-145">応答</span><span class="sxs-lookup"><span data-stu-id="ae1e6-145">Response</span></span>
<span data-ttu-id="ae1e6-146">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae1e6-147">例</span><span class="sxs-lookup"><span data-stu-id="ae1e6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae1e6-148">要求</span><span class="sxs-lookup"><span data-stu-id="ae1e6-148">Request</span></span>
<span data-ttu-id="ae1e6-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="ae1e6-150">応答</span><span class="sxs-lookup"><span data-stu-id="ae1e6-150">Response</span></span>
<span data-ttu-id="ae1e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae1e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




