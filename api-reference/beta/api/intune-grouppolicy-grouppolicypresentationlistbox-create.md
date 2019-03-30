---
title: grouppolicypresentationlistbox の作成
description: 新しい grouppolicypresentationlistbox オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e57fa0a5ce0f4bbaa3bd9a50383a6c7505083cf4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979418"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="31476-103">grouppolicypresentationlistbox の作成</span><span class="sxs-lookup"><span data-stu-id="31476-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="31476-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31476-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31476-106">新しい[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31476-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31476-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="31476-107">Prerequisites</span></span>
<span data-ttu-id="31476-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31476-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31476-110">Permission type</span></span>|<span data-ttu-id="31476-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31476-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31476-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31476-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31476-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31476-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31476-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31476-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31476-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31476-115">Not supported.</span></span>|
|<span data-ttu-id="31476-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31476-116">Application</span></span>|<span data-ttu-id="31476-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31476-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31476-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31476-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="31476-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31476-119">Request headers</span></span>
|<span data-ttu-id="31476-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31476-120">Header</span></span>|<span data-ttu-id="31476-121">値</span><span class="sxs-lookup"><span data-stu-id="31476-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31476-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31476-122">Authorization</span></span>|<span data-ttu-id="31476-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31476-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31476-124">承諾</span><span class="sxs-lookup"><span data-stu-id="31476-124">Accept</span></span>|<span data-ttu-id="31476-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31476-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31476-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="31476-126">Request body</span></span>
<span data-ttu-id="31476-127">要求本文で、grouppolicypresentationlistbox オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31476-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="31476-128">次の表に、grouppolicypresentationlistbox の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31476-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="31476-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31476-129">Property</span></span>|<span data-ttu-id="31476-130">型</span><span class="sxs-lookup"><span data-stu-id="31476-130">Type</span></span>|<span data-ttu-id="31476-131">説明</span><span class="sxs-lookup"><span data-stu-id="31476-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31476-132">label</span><span class="sxs-lookup"><span data-stu-id="31476-132">label</span></span>|<span data-ttu-id="31476-133">String</span><span class="sxs-lookup"><span data-stu-id="31476-133">String</span></span>|<span data-ttu-id="31476-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="31476-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="31476-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="31476-135">The default value is empty.</span></span> <span data-ttu-id="31476-136">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="31476-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31476-137">id</span><span class="sxs-lookup"><span data-stu-id="31476-137">id</span></span>|<span data-ttu-id="31476-138">String</span><span class="sxs-lookup"><span data-stu-id="31476-138">String</span></span>|<span data-ttu-id="31476-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31476-139">Key of the entity.</span></span> <span data-ttu-id="31476-140">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="31476-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31476-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31476-141">lastModifiedDateTime</span></span>|<span data-ttu-id="31476-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31476-142">DateTimeOffset</span></span>|<span data-ttu-id="31476-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="31476-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="31476-144">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="31476-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="31476-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="31476-145">explicitValue</span></span>|<span data-ttu-id="31476-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="31476-146">Boolean</span></span>|<span data-ttu-id="31476-147">このオプションが指定されている場合、ユーザーはレジストリサブキーの値とレジストリサブキー名を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="31476-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="31476-148">リストボックスに2つの列が表示されます。1つは名前用、もう1つはデータ用です。</span><span class="sxs-lookup"><span data-stu-id="31476-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="31476-149">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="31476-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="31476-150">応答</span><span class="sxs-lookup"><span data-stu-id="31476-150">Response</span></span>
<span data-ttu-id="31476-151">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31476-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31476-152">例</span><span class="sxs-lookup"><span data-stu-id="31476-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="31476-153">要求</span><span class="sxs-lookup"><span data-stu-id="31476-153">Request</span></span>
<span data-ttu-id="31476-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31476-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="31476-155">応答</span><span class="sxs-lookup"><span data-stu-id="31476-155">Response</span></span>
<span data-ttu-id="31476-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31476-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




