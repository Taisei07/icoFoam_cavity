/*--------------------------------*- C++ -*----------------------------------*\
| =========                 |                                                 |
| \\      /  F ield         | OpenFOAM: The Open Source CFD Toolbox           |
|  \\    /   O peration     | Version:  5                                     |
|   \\  /    A nd           | Web:      www.OpenFOAM.org                      |
|    \\/     M anipulation  |                                                 |
\*---------------------------------------------------------------------------*/
FoamFile
{
    version     2.0;
    format      ascii;
    class       volScalarField;
    object      p;//圧力の境界条件設定
}
// * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * //

dimensions      [0 2 -2 0 0 0 0];//単位はm^2/s^2

internalField   uniform 0;

boundaryField
{
    fixedWalls
    {
        type            zeroGradient;
    }

    inlet
    {
        type            zeroGradient;
    }

    outlet
    {
        type            fixedValue;
        value           uniform 101325;
    }
    frontAndBack
    {
        type            empty;
    }
}
//新しく作った境界条件（fixedWalls・inlet・outlet・frontAndBack）
/*前のやつ
movingWall
{
    type            zeroGradient;
}

fixedWalls
{
    type            zeroGradient;
}

frontAndBack//inletとoutletが必要？
{
    type            empty;
}

// ************************************************************************* //
