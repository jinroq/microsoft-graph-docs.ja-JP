---
title: registryKeyState リソースの種類
description: アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067144"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="b7044-103">registryKeyState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7044-103">registryKeyState resource type</span></span>

<span data-ttu-id="b7044-104">アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7044-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="b7044-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7044-105">Properties</span></span>

| <span data-ttu-id="b7044-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7044-106">Property</span></span>     | <span data-ttu-id="b7044-107">型</span><span class="sxs-lookup"><span data-stu-id="b7044-107">Type</span></span>        | <span data-ttu-id="b7044-108">説明</span><span class="sxs-lookup"><span data-stu-id="b7044-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7044-109">ハイブ</span><span class="sxs-lookup"><span data-stu-id="b7044-109">hive</span></span>|<span data-ttu-id="b7044-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="b7044-110">registryHive</span></span>|<span data-ttu-id="b7044-111">[Windows レジストリ ハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)。</span><span class="sxs-lookup"><span data-stu-id="b7044-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="b7044-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="b7044-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="b7044-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="b7044-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="b7044-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="b7044-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="b7044-115">\Security</span><span class="sxs-lookup"><span data-stu-id="b7044-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="b7044-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="b7044-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="b7044-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="b7044-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="b7044-118">HKEY_USERS\\。既定値です。</span><span class="sxs-lookup"><span data-stu-id="b7044-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="b7044-119">可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault` です。</span><span class="sxs-lookup"><span data-stu-id="b7044-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="b7044-120">Key</span><span class="sxs-lookup"><span data-stu-id="b7044-120">key</span></span>|<span data-ttu-id="b7044-121">String</span><span class="sxs-lookup"><span data-stu-id="b7044-121">String</span></span>|<span data-ttu-id="b7044-122">現在の (変更されているなど) のレジストリ キー (ハイブを除く)。</span><span class="sxs-lookup"><span data-stu-id="b7044-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="b7044-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="b7044-123">oldKey</span></span>|<span data-ttu-id="b7044-124">String</span><span class="sxs-lookup"><span data-stu-id="b7044-124">String</span></span>|<span data-ttu-id="b7044-125">(つまり変更前に) は、以前のレジストリ キー (ハイブを除く)。</span><span class="sxs-lookup"><span data-stu-id="b7044-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="b7044-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="b7044-126">oldValueData</span></span>|<span data-ttu-id="b7044-127">String</span><span class="sxs-lookup"><span data-stu-id="b7044-127">String</span></span>|<span data-ttu-id="b7044-128">以前の (つまり変更前に) レジストリ キーの値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="b7044-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="b7044-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="b7044-129">oldValueName</span></span>|<span data-ttu-id="b7044-130">String</span><span class="sxs-lookup"><span data-stu-id="b7044-130">String</span></span>|<span data-ttu-id="b7044-131">以前の (つまり変更前に) レジストリ キーの値の名前。</span><span class="sxs-lookup"><span data-stu-id="b7044-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="b7044-132">操作​​</span><span class="sxs-lookup"><span data-stu-id="b7044-132">operation</span></span>|<span data-ttu-id="b7044-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="b7044-133">registryOperation</span></span>|<span data-ttu-id="b7044-134">レジストリ キーの名前または値を変更する操作です。</span><span class="sxs-lookup"><span data-stu-id="b7044-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="b7044-135">可能な値は、`unknown`、`create`、`modify`、`delete` です。</span><span class="sxs-lookup"><span data-stu-id="b7044-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="b7044-136">プロセス Id</span><span class="sxs-lookup"><span data-stu-id="b7044-136">processId</span></span>|<span data-ttu-id="b7044-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b7044-137">Int32</span></span>|<span data-ttu-id="b7044-138">(プロセスのアラート 'プロセス' コレクションの詳細が表示されます) のレジストリ キーを変更するプロセスの ID (PID) を処理します。</span><span class="sxs-lookup"><span data-stu-id="b7044-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="b7044-139">セグ</span><span class="sxs-lookup"><span data-stu-id="b7044-139">valueData</span></span>|<span data-ttu-id="b7044-140">String</span><span class="sxs-lookup"><span data-stu-id="b7044-140">String</span></span>|<span data-ttu-id="b7044-141">現在 (つまり変更されている) のレジストリ キーの値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="b7044-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="b7044-142">値名</span><span class="sxs-lookup"><span data-stu-id="b7044-142">valueName</span></span>|<span data-ttu-id="b7044-143">String</span><span class="sxs-lookup"><span data-stu-id="b7044-143">String</span></span>|<span data-ttu-id="b7044-144">現在の (変更されているなど) のレジストリ キー値の名前</span><span class="sxs-lookup"><span data-stu-id="b7044-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="b7044-145">valueType</span><span class="sxs-lookup"><span data-stu-id="b7044-145">valueType</span></span>|<span data-ttu-id="b7044-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="b7044-146">registryValueType</span></span>|[<span data-ttu-id="b7044-147">レジストリ キーの値の型</span><span class="sxs-lookup"><span data-stu-id="b7044-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="b7044-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="b7044-148">REG_BINARY</span></span></li> <li><span data-ttu-id="b7044-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b7044-149">REG_DWORD</span></span></li> <li><span data-ttu-id="b7044-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b7044-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="b7044-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b7044-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="b7044-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="b7044-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="b7044-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="b7044-153">REG_LINK</span></span></li> <li><span data-ttu-id="b7044-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="b7044-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="b7044-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="b7044-155">REG_NONE</span></span></li> <li><span data-ttu-id="b7044-156">定義</span><span class="sxs-lookup"><span data-stu-id="b7044-156">REG_QWORD</span></span></li> <li><span data-ttu-id="b7044-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="b7044-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="b7044-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="b7044-158">REG_SZ</span></span></li></ul> <span data-ttu-id="b7044-159">可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。</span><span class="sxs-lookup"><span data-stu-id="b7044-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7044-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7044-160">JSON representation</span></span>

<span data-ttu-id="b7044-161">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7044-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->